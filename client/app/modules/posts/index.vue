<template>
	<div class="container">
		<div class="row">
			<div class="col">
				<h2 class="title">{{ _('Posts') }}</h2>
			</div>
		</div>
		<div class="row py-3">
			<div class="col">	
				<div class="group sort">
					<a class="btn btn-light" role="button" @click="changeSort('-votes')" :class="{ active: sort == '-votes' }">{{ _("Hot") }}</a>
					<a class="btn btn-light" role="button" @click="changeSort('-views')" :class="{ active: sort == '-views' }">{{ _("MostViewed") }}</a>
					<a class="btn btn-light" role="button" @click="changeSort('-createdAt')" :class="{ active: sort == '-createdAt' }">{{ _("New") }}</a>
				</div>
			</div>
			<div class="col d-flex justify-content-center">
				<button class="btn btn-light" @click="newPost">
					<span class="icon"><i class="fas fa-plus"></i></span>
					<span>{{ _("NewPost") }}</span>
				</button>	
			</div>
			<div class="col d-flex justify-content-end">
				<a class="btn btn-light" @click="changeViewMode('all')" :class="{ active: viewMode == 'all' }">{{ _("AllPosts") }}</a>
				<a class="btn btn-light" @click="changeViewMode('my')" :class="{ active: viewMode == 'my' }">{{ _("MyPosts") }}</a>
			</div>
		</div>
		
		<div class="row">
			<div class="col">
				<div class="postForm" v-if="showForm">
					<vue-form-generator :schema="schema" :model="model" :options="{}" :multiple="false" ref="form" :is-new-model="isNewPost"></vue-form-generator>
					<div class="group buttons">
						<button class="btn btn-primary" @click="savePost">{{ _("Save") }}</button>
						<button class="btn btn-secondary" @click="cancelPost">{{ _("Cancel") }}</button>
					</div>
				</div>
			</div>
		</div>

		<div class="row">
			<div class="col">
				<transition-group class="posts" name="post" tag="div">
					<div v-for="post of posts" :key="post.code">
						<div class="card">
							<h5 class="card-header">{{ post.title }}</h5>
							<div class="row">
								<div class="col-1 py-3 px-4">
									<div class="media-left"><img class="avatar" :src="post.author.avatar" />
										<div class="votes" :class="{ voted: iVoted(post) }">
											<div class="count text-center">{{ post.votes }}</div>
											<div class="thumb text-center" @click="toggleVote(post)"><i class="fas fa-thumbs-up"></i></div>
										</div>
									</div>			
								</div>
								<div class="col">
									<div class="card-body">
										<div class="row">
											<div class="col">
												<p class="content" v-html="markdown(post.content)"></p>
												<hr/>
											</div>
										</div>
										<div class="row">
											<div class="col">
												<div class="float-left"><a :title="_('EditPost')" @click="editPost(post)">
													<i class="fas fa-edit"></i></a><a :title="_('DeletePost')" @click="deletePost(post)">
													<i class="fas fa-trash"></i></a>
												</div>
												<div class="flex-row" :title="_('Voters')">
													<template v-for="voter in lastVoters(post)">
														<img :src="voter.avatar" :title="voter.fullName + ' (' + voter.username + ')'"/>
													</template>
												</div>
												
											</div>
											<div class="col">
												<div class="right text-right">
													<template v-if="post.editedAt">
														<small class="text-muted">{{ editedAgo(post) }}</small><br/>
													</template>
													<small class="text-muted">{{ createdAgo(post) }}</small>
												</div>
											</div>
										</div>
									</div>
								</div>
							</div>
						</div>
					</div>
				</transition-group>
			</div>
		</div>

		<div class="loadMore text-center" v-if="hasMore">
			<button class="btn btn-primary" @click="loadMoreRows" :class="{ 'loading': fetching }">{{ _("LoadMore") }}</button>
		</div>
		<div class="noMore text-center" v-if="!hasMore"><span class="text-muted">You reached the end of the list.</span></div>
		<hr/>
	</div>
</template>

<script>
	import Vue from "vue";
	import marked from "marked";
	import toast from "../../core/toastr";
	import { cloneDeep } from "lodash";
	import { validators, schema as schemaUtils } from "vue-form-generator";
	import { mapGetters, mapActions } from "vuex";

	export default {

		computed: {
			...mapGetters("posts", [
				"posts",
				"hasMore",
				"fetching",
				"sort",
				"viewMode"
			]),
			...mapGetters("session", [
				"me"
			])
		},

		/**
		 * Set page schema as data property
		 */
		data() {
			return {
				showForm: false,
				isNewPost: false,
				model: null,
				schema: {
					fields: [
						{
							type: "input",
							label: this._("Title"),
							model: "title",
							featured: true,
							required: true,
							placeholder: this._("TitleOfPost"),
							validator: validators.string
						},
						{
							type: "textArea",
							label: this._("Content"),
							model: "content",
							featured: true,
							required: true,
							rows: 10,
							placeholder: this._("ContentOfPost"),
							validator: validators.string
						}
					]
				}
			};
		},

		/**
		 * Socket handlers. Every property is an event handler
		 */
		socket: {

			prefix: "/posts/",

			events: {
				/**
				 * New device added
				 * @param  {Object} res Device object
				 */
				/*
				We don't use it because we don't know we need to add it to the page (filter, sort..etc)
				created(res) {
					this.created(res.data);
					toast.success(this._("PostNameAdded", res), this._("PostAdded"));
				},*/

				/**
				 * Post updated
				 * @param  {Object} res Post object
				 */
				updated(res) {
					this.updated(res.data);
					toast.success(this._("PostNameUpdated", res), this._("PostUpdated"));
				},

				voted(res) {
					this.updated(res.data);
					toast.success(this._("PostNameVoted", res), this._("PostUpdated"));
				},

				unvoted(res) {
					this.updated(res.data);
					toast.success(this._("PostNameUnvoted", res), this._("PostUpdated"));
				},

				/**
				 * Post removed
				 * @param  {Object} res Post object
				 */
				removed(res) {
					this.removed(res.data);
					toast.success(this._("PostNameDeleted", res), this._("PostDeleted"));
				}
			}
		},

		methods: {
			...mapActions("posts", [
				"getRows",
				"loadMoreRows",
				"changeSort",
				"changeViewMode",
				"vote",
				"unVote",
				"saveRow",
				"updateRow",
				"removeRow",
				"updated",
				"removed"
			]),

			markdown(content) {
				return marked(content);
			},

			iVoted(post) {
				return _.find(post.voters, (user) => user.code == this.me.code) != null;
			},

			toggleVote(post) {
				if (this.iVoted(post))
					this.unVote(post);
				else
					this.vote(post);
			},

			lastVoters(post, count = 5) {
				if (post.voters && post.voters.length > 0) {
					let voters = _.clone(post.voters).reverse().slice(0, 5);
					return voters;
				}
				return [];
			},

			createdAgo(post) {
				return this._("CreatedAgoByName", { ago: Vue.filter("ago")(post.createdAt), name: post.author.fullName } );
			},

			editedAgo(post) {
				if (post.editedAt)
					return this._("EditedAgo", { ago: Vue.filter("ago")(post.editedAt) } );
			},

			newPost() {
				this.model = schemaUtils.createDefaultObject(this.schema);
				this.showForm = true;
				this.isNewPost = true;

				this.focusFirstInput();
			},

			editPost(post) {
				this.model = cloneDeep(post);
				this.showForm = true;
				this.isNewPost = false;
				this.focusFirstInput();
			},

			focusFirstInput() {
				this.$nextTick(() => {
					let el = document.querySelector(".postForm .form-control:nth-child(1):not([readonly]):not(:disabled)");
					if (el)
						el.focus();
				});
			},

			focusFirstErrorInput() {
				this.$nextTick(() => {
					let el = document.querySelector(".postForm .form-group.error .form-control");
					if (el)
						el.focus();
				});
			},

			savePost() {
				if (this.$refs.form.validate()) {
					if (this.isNewPost)
						this.saveRow(this.model);
					else
						this.updateRow(this.model);

					this.cancelPost();
				} else {
					this.focusFirstErrorInput();
				}
			},

			cancelPost() {
				this.showForm = false;
				this.model = null;
			},

			deletePost(post) {
				this.removeRow(post);
			}

		},

		/**
		 * Call if the component is created
		 */
		created() {
			this.getRows();
		}
	};
</script>

<style lang="scss" scoped>
</style>