<template>
	<h3>Watch </h3>
	<button @click="changeText">Change</button>
	<p>{{ message }}</p>
</template>
<script>
export default {
	data() {
		return {
			message: "test"
		}
	},
	methods: {
		changeText() {
			// console.log('Old:' + this.message);
			this.message = "Hello" + "H"
		}
	},
	watch: {
		message(newValue, oldValue) {
			console.log(oldValue + newValue)
		}
	}
}
</script>