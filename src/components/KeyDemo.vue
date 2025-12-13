<template>
	<h3>Key Demo</h3>
	<div>
		<h4>nokey</h4>
		<p v-for="(item, index) of names">{{ item }}</p>
	</div>
	<div>
		<h4>withkey</h4>
		<p v-for="(item, index) of users" :id="item.id">{{ item.username }}</p>
	</div>
</template>

<script>
export default {
	data() {
		return {
			names: ['anan', 'tian', 'cheng'],
			users: [
				{
					id: 1,
					username: "anan",
				},
				{
					id: 2,
					username: "tiantian",
				},
				{
					id: 3,
					username: "chengcheng",
				},
			]
		}
	}
}
</script>