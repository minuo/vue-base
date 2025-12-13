<template>
	<h3>事件修饰符</h3>
	<a @click.prevent="clickHandle" href="http://minuo.org">minuo.org</a>

	<div @click="clickDiv">
		<p @click.stop="clickP">内部</p>
	</div>
</template>

<script>
export default {
	methods: {
		clickHandle() {
			console.log('asde')
		},
		clickDiv() {
			console.log("div");
		},
		clickP() {
			console.log("p")
		}
	}
}
</script>

<style scoped>
div {
	background-color: rebeccapurple;
}
</style>