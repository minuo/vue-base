<template>
	<h2>Event with params</h2>

	<p @click="GetNameHander(item, $event)" v-for="item of names">{{ item }}</p>

</template>
<script>
export default {
	data() {
		return {
			names: ['anan', 'tian', 'cheng']
		}
	},
	methods: {
		GetNameHander(name, e) {
			// get data 
			console.log(name);
			console.log(e);
		}
	}
}
</script>