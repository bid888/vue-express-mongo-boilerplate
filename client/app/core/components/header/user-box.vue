<template>
	<ul class="navbar-nav flex-row d-none d-md-flex">
		<li :class=" { active: notifications.length &gt; 0 }" class="nav-item dropdown" v-if="me">
			<a class="user-info right nav-link dropdown-toggle p-2 text-secondary" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" @click="toggleNotifications()">
				<i class="far fa-bell"></i><span>{{ " " + notifications.length }}</span>
			</a>
			<notifications-dropdown></notifications-dropdown>
		</li>
		
		<li :class=" { active: messages.length &gt; 0 }" class="nav-item dropdown" v-if="me">
			<a class="user-info right nav-link dropdown-toggle p-2 text-secondary" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" @click="toggleMessages()">
				<i class="far fa-envelope"></i><span>{{ " " + messages.length }}</span>
			</a>
			<messages-dropdown></messages-dropdown>
		</li>
		<li class="nav-item dropdown" v-if="me">
			<a class="user-info right nav-link dropdown-toggle p-2 text-secondary" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" @click="toggleUserMenu()">
				<img width="30" height="30" class="avatar d-inline-block align-top" :src="me.avatar" />
				{{ me.fullName }}
			</a>
			<user-dropdown></user-dropdown>
		</li>
	</ul>
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