<template>
	<h3>表单输入绑定</h3>
	<input type="text" v-model="message">

	<p>{{ message }}</p>


	<input type="checkbox" name="CheckBox" id="checkbox" v-model="checked">
	<label for="checkbox">{{ checked }}</label>
</template>
<script>
export default {
	data() {
		return {
			message: "",
			checked: false
		}
	}
}
</script>