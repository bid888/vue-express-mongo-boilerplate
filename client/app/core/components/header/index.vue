<template>
	<nav class="navbar navbar-expand-lg navbar-light bg-white rounded">
		<div class="container">
			<a class="navbar-brand" href="#">
				<img src="https://getbootstrap.com/docs/4.3/assets/brand/bootstrap-solid.svg" width="30" height="30" class="d-inline-block align-top" alt="">
			</a>
			<button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarsExample10" aria-controls="navbarsExample10" aria-expanded="false" aria-label="Toggle navigation">
				<span class="navbar-toggler-icon"></span>
			</button>

			<ul class="navbar-nav">
				<router-link tag="li" to="/counter" class="nav-item active"><a class="nav-link" :title="_('Demo')"><span class="icon"><i class="fa fa-tasks"></i></span><span class="label">{{ "Demo" | i18n }}</span></a></router-link>
				<router-link tag="li" to="/devices" class="nav-item active"><a class="nav-link" :title="_('Devices')"><span class="icon"><i class="fa fa-tablet"></i></span><span class="label">{{ "Devices" | i18n }}</span></a></router-link>
				<router-link tag="li" to="/posts" class="nav-item active"><a class="nav-link" :title="_('Posts')"><span class="icon"><i class="fa fa-comments"></i></span><span class="label">{{ "Posts" | i18n }}</span></a></router-link>
			</ul>

			<div>
				<div class="navbar-collapse collapse show" id="navbarsExample10">
					<ul class="navbar-nav">
						<search-box></search-box>	
						<user-box></user-box>
					</ul>
				</div>
			</div>
			
		</div>
	</nav>
</template>

<script>
	import SearchBox from "./search-box";
	import UserBox from "./user-box";

	export default {
		components: {
			SearchBox,
			UserBox
		},

		props: [
			"toggleSidebar"
		]

	};
	
</script>

<style lang="scss">
	.navbar {
		margin-bottom: 20px;
	}

	.container {
		padding: 0 !important;
	}
</style>