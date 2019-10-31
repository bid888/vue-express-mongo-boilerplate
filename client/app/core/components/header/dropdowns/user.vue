<template>
	<div class="dropdown-menu dropdown-menu-right">
		<router-link tag="li" to="/profile">
			<a class="dropdown-item"><span class="icon"><i class="fa fa-user"></i></span>{{ " My Account" | i18n }}</a>
		</router-link>
		<router-link tag="li" to="/settings">
			<a class="dropdown-item"><span class="icon"><i class="fa fa-cog"></i></span>{{ " Settings" | i18n }}</a>
		</router-link>
		<div class="dropdown-divider"></div>
		<li>
			<a class="dropdown-item" href="/logout"><span class="icon"><i class="fa fa-power-off"></i></span>{{ " Logout" | i18n }}</a>
		</li>
	</div>	
</template>

<script>
	export default {
		props: [
			"visible"
		]
	};	
</script>

<style lang="scss">
</style>