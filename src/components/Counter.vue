<template>
	<div class="">
		<button @click="increment">+</button>
		<button @click="decrement">-</button>
		<p><span>{{ num }}</span></p>
		
	</div>
</template>

<script>
	export default {
		props:['num'],
		data() {
			return {
				msg: 'Welcome to Your Vue.js App',
				
			}
		},
		methods: {
			increment() {
				this.$emit('incre')
			},
			decrement() {
				this.$emit('decre')
			}
		}
	}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>