<template>
	<div class="container h-100">
		<div class="row py-4">
			<div class="col">
				<h1 class="title py-2">{{ "Demo" | i18n }}</h1>
				<h3 class="py-2">Counter: {{ count }}</h3>
				<div class="py-2">
					<button type="button" class="btn btn-primary" @click="inc"><span class="icon"><i class="fas fa-arrow-up"></i></span><span>{{ " Increment" | i18n }}</span>
					</button>
					<button type="button" class="btn btn-primary" @click="dec"><span><i class="fas fa-arrow-down"></i></span><span>{{ " Decrement" | i18n }}</span>
					</button>
				</div>
			</div>
		</div>	
	</div>
</template>

<script>
	import { mapActions, mapGetters } from "vuex";

	import Service from "../../core/service";

	export default {
		/**
		 * Computed getters
		 */
		 computed: mapGetters("counter", [
			 "count"
		 ]),

		/**
		 * Page methods
		 */
		methods: {
			/**
			 * Actions from store
			 */
			...mapActions("counter", [
				"getValue",
				"increment",
				"decrement",
				"changedValue"
			]),

			/**
			 * Increment counter
			 */
			inc() {
				this.increment();
			},

			/**
			 * Decrement counter
			 */
			dec() {
				this.decrement();
			}
		},

		/**
		 * Socket handlers. Every property is an event handler
		 */
		socket: {

			prefix: "/counter/",

			//namespace: "/counter",

			events: {
				/**
				 * Counter value is changed
				 * @param  {Number} msg Value of counter
				 */
				changed(res) {
					console.log("Counter changed to " + res.data + (res.user ? " by " + res.user.fullName : ""));
					this.changedValue(res.data);
				}
			}
		},

		created() {
			this.$service = new Service("counter", this); 
			
			// Get the latest value of counter
			this.getValue(); 
		}
	};

</script>

<style lang="scss" scoped>
</style>