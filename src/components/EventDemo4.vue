<template>
	<h2>Event demo 3</h2>
	<button @click="addCount('hello')">ADD</button>
	<p>{{ count }}</p>
</template>
<script>
export default {
	data() {
		return {
			count: 1
		}
	},
	methods: {
		addCount(msg) {
			// get data 
			console.log(msg);
			this.count++
		}
	}
}
</script>