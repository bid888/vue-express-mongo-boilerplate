<template>
	<div class="container">
		<div class="row py-3">
			<div class="col-1">
				<div class="profile flex row align-stretch"><img class="avatar" :src="profile.avatar" />
				</div>
			</div>
			<div class="col">
				<div class="details flex-item-1">
					<h3 class="name font-weight-bolder">{{ profile.fullName }}<span class="text-muted username"> ({{ profile.username }})</span></h3>
					<div class="tags">
						<div class="badge badge-primary">!Role name!</div>
						<div class="badge badge-secondary">!Administrator!</div>
						<div class="badge badge-success">!Online!</div>
					</div>
					<div class="description py-2">
						<div class="info-row" v-if="profile.profile &amp;&amp; profile.profile.location"><i class="fa fa-map-marker"></i><span class="caption">Location:</span><span class="value"> {{ profile.profile.location }}</span></div>
						<div class="info-row py-1"><i class="fas fa-history"></i><span class="caption"> Last login:</span><span class="value"> !Online!</span></div>
						<div class="info-row py-1"><i class="far fa-calendar-alt"></i><span class="caption"> Joined:</span><span class="value"> {{ profile.createdAt | ago }}</span></div>
					</div>
					<hr class="full" />
				</div>
			</div>
		</div>
		<div class="row">
			<div class="col-1">
			</div>
			<div class="col">
				<pre v-html="this.$options.filters.prettyJSON(profile)"></pre>
			</div>
		</div>
	</div>
</template>

<script>
	import Service from "../../core/service";
	import { mapGetters, mapActions } from "vuex";

	export default {
		computed: mapGetters("profile", [
			"profile"
		]),

		methods: {
			...mapActions("profile", [
				"getProfile"
			])
		},

		created() {
			this.$service = new Service("profile", this); 
			this.getProfile(); 
		}
	};
</script>

<style lang="scss" scoped>
</style>