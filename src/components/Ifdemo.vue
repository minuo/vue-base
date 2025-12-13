<template>
	<div v-bind:class="cls" v-bind:id="cid">{{ text }}</div>
	<button :disabled="isBtnDisabled">Button</button>
	<div v-bind="objAttr">Newtest</div>

	<div v-if="flag"> flag is true, you can see me.</div>
	<div v-if="flagfalse"> flag is false, you can't see me.</div>

	<div v-show="flag">v-show, you can see me</div>


</template>


<script>
export default {
	data() {
		return {
			cls: "active",
			cid: "no-active",
			title: "",
			text: "hello world",
			isBtnDisabled: true,
			objAttr: {
				id: "customId",
				class: "customClass",
			},
			flag: true,
			flagfalse: false,
		}
	}
}
</script>
<style scoped></style>
