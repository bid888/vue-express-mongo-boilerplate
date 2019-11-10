<template>
	<div class="notification-dropdown dropdown-menu" style="padding:0">
		<div class="card" style="width: 30rem;">
			<div class="card-header">
				<div class="header">
					<div class="row">
						<div class="col-9">
							{{ "Notifications" | i18n }}
						</div>
						<div class="col-3">
							<a class="link" href="#"> <small>{{ "MarkAllAsRead" | i18n }}</small></a>
						</div>
					</div>
				</div>
			</div>
			<ul class="list-group list-group-flush">
				<li class="list-group-item">
					<div class="row">
						<div class="col-2">
							<img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/dustin/73.jpg" />
						</div>
						<div class="col-7">
							<p> <strong>Thomas </strong>posted a new article</p>
						</div>
						<div class="col-3">
							<small class="text-muted">1 min ago</small>
						</div>
					</div>
				</li>
				<li class="list-group-item">
					<div class="row">
						<div class="col-2">
							<img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/connor_gaunt/73.jpg" />
						</div>
						<div class="col-7">
							<p> <strong>Adam </strong>changed his contact information</p>
						</div>
						<div class="col-3">
							<small class="text-muted">3 min ago</small>
						</div>
					</div>
				</li>
				<li class="list-group-item">
					<div class="row">
						<div class="col-2">
							<img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/adellecharles/73.jpg" />
						</div>
						<div class="col-7">
							<p> <strong>Samantha </strong>replied to your comment</p>
						</div>
						<div class="col-3">
							<small class="text-muted">15 min ago</small>
						</div>
					</div>
				</li>
				<li class="list-group-item">	
					<div class="row">
						<div class="col-2">
							<img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/ritu/73.jpg" />
						</div>
						<div class="col-7">
							<p class="text-justify"> <strong>Bill </strong>bought a new TV</p>
						</div>
						<div class="col-3">
							<small class="text-muted">3 hours ago</small>
						</div>
					</div>
				</li>
				<li class="list-group-item">
					<div class="row">
						<div class="col-2">
							<img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/sauro/73.jpg" />
						</div>
						<div class="col-7">
							<p> <strong>Chris </strong>posted a new blog post</p>
						</div>
						<div class="col-3">
							<small class="text-muted">1 day ago</small>
						</div>
					</div>
				</li>
			</ul>
			<div class="footer text-center"><a class="link" href="#">{{ "SeeAllNotifications" | i18n }}</a></div>
		</div>
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