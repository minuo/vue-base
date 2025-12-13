<template>
	<h2>Event demo 1</h2>
	<button @click="count++">count:{{ count }}</button>
</template>
<script>
export default {
	data() {
		return {
			count: 0
		}
	}
}
</script>