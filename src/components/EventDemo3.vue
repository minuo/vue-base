<template>
	<h2>Event demo 3</h2>
	<button @click="addCount">ADD</button>
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
		addCount(e) {
			// get data 
			// console.log(e);
			e.target.innerHTML = "asdf" + this.count;
			this.count++
		}
	}
}
</script>