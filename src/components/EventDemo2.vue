<template>
	<h2>Event demo 2</h2>
	<button @mouseover="addCount">count:{{ count }}</button>
</template>
<script>
export default {
	data() {
		return {
			count: 1
		}
	},
	methods: {
		addCount() {
			// get data 
			this.count++
		}
	}
}
</script>