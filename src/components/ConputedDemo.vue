<template>
	<h3>计算属性</h3>

	<p>{{ postContent }}</p>
</template>

<script>
export default {
	data() {
		return {
			post: {
				id: 1,
				title: "test title for frontend, content is an array",
				content: ['asd', 'esf', 'ech']
			}
		}
	},
	computed: {
		postContent() {
			return this.post.content.length > 0 ? '<p>' + this.post.content + '</p>' : "no content"
		}
	}
}
</script>