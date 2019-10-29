<template>
	<div class="collapse navbar-collapse">
		<ul class="navbar-nav mr-auto">
			<li :class=" { active: notifications.length &gt; 0 }" class="nav-item dropdown" v-if="me">
				<a class="user-info right nav-link dropdown-toggle" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" @click="toggleNotifications()">
					<i class="fas fa-bell"></i><span>{{ notifications.length }}</span>
				</a>
				<notifications-dropdown></notifications-dropdown>
			</li>
			
			<li :class=" { active: messages.length &gt; 0 }" class="nav-item dropdown" v-if="me">
				<a class="user-info right nav-link dropdown-toggle" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" @click="toggleMessages()">
					<i class="fas fa-envelope"></i><span>{{ messages.length }}</span>
				</a>
				<messages-dropdown></messages-dropdown>
			</li>
			<li class="nav-item dropdown" v-if="me">
				<a class="user-info right nav-link dropdown-toggle" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" @click="toggleUserMenu()">
					<img width="30" height="30" class="avatar d-inline-block align-top" :src="me.avatar" />
					{{ me.fullName }}
				</a>
				<user-dropdown></user-dropdown>
			</li>
		</ul>
	</div>

	<!-- <div class="notification-box right">
			<ul class="icons">
				<li @click="toggleNotifications()" :class=" { active: notifications.length &gt; 0 }"><i class="fa fa-bell-o"></i><span>{{ notifications.length }}</span>
					<div class="ring"></div>
				</li>
				<li @click="toggleMessages()" :class=" { active: messages.length &gt; 0 }"><i class="fa fa-envelope-o"></i><span>{{ messages.length }}</span>
					<div class="ring"></div>
				</li>
			</ul>
			<notifications-dropdown :visible="expandedNotifications"></notifications-dropdown>
			<messages-dropdown :visible="expandedMessages"></messages-dropdown>
		</div> -->
</template>

<script>
	import UserDropdown from "./dropdowns/user";
	import NotificationsDropdown from "./dropdowns/notifications";
	import MessagesDropdown from "./dropdowns/messages";

	import { mapActions, mapGetters } from "vuex";

	export default {
		computed: mapGetters("session", [
			"me",
			"notifications",
			"messages"
		]),

		components: {
			UserDropdown,
			NotificationsDropdown,
			MessagesDropdown
		},

		data() {
			return {
				expandedUserMenu: false,
				expandedNotifications: false,
				expandedMessages: false
			};
		},

		methods: {
			toggleUserMenu() {
				this.expandedUserMenu = !this.expandedUserMenu;
				if (this.expandedUserMenu) {
					this.expandedMessages = false;
					this.expandedNotifications = false;
				}
			},

			toggleMessages() {
				this.expandedMessages = !this.expandedMessages;
				if (this.expandedMessages) {
					this.expandedUserMenu = false;
					this.expandedNotifications = false;
				}
			},

			toggleNotifications() {
				this.expandedNotifications = !this.expandedNotifications;
				if (this.expandedNotifications) {
					this.expandedMessages = false;
					this.expandedUserMenu = false;
				}
			}
		}
	};
</script>

<style lang="scss">
</style>