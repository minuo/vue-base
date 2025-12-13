<template>

	<h3>数组变化监测</h3>
	<p @click="addEle" v-for="item in names">{{ item }}</p>
</template>

<script>
export default {
	data() {
		return {
			names: ['anan', "tian", 'cheng']
		}
	},
	methods: {
		addEle() {
			this.names.push("aaa")
			// this.names.concat(["aaa"])

			// console.log(this.names.concat(["aaa"]))

		}
	}
}
</script>