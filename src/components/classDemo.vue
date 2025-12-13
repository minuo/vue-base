<template>
	<h3>Class 绑定</h3>
	<p :class="{ 'active': isActive, 'text-danger': warning }">Demo</p>
	<p :class="classObj">Demo2</p>
</template>

<script>
export default {
	data() {
		return {
			isActive: true,
			warning: false,
			classObj: {
				'active': true,
				'text-danger': false,
			}
		}
	}
}
</script>


<style scoped>
.active {
	border: 1px solid red;
	padding: 1rem;
}

.text-danger {
	color: red;
	background-color: rebeccapurple;
}
</style>