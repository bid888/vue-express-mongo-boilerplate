<template>
	<form class="form-inline mt-2 mt-md-0">
		<i class="fa fa-search"></i>
		<input class="form-control mr-sm-2" v-model="text" :placeholder="_('Search3dots')" type="search" aria-label="Search">
		<button class="btn btn-outline-info my-2 my-sm-0" type="submit">Search</button>
	</form>
</template>

<script>
	import { mapGetters, mapActions } from "vuex";

	export default {
		computed: {
			...mapGetters("session", [
				"searchText"
			]),
			text: {
				get() {
					return this.searchText;
				},

				set(value) {
					this.searching(value);
				}
			}
		},

		methods: {
			...mapActions("session", [
				"searching"
			])
		}
	};	
</script>

<style lang="scss">
</style>