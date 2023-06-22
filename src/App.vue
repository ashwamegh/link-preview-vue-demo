<template>
	<div id="app">
		<LinkPreview url="https://vuejs.org/" @click="handleClick"></LinkPreview>
	</div>
</template>

<script>
import LinkPreview from "@ashwamegh/vue-link-preview";

export default {
	name: "App",
	components: {
		LinkPreview,
	},
	methods: {
		handleClick(preview) {
			console.log(
				"click",
				preview.domain,
				preview.title,
				preview.description,
				preview.img
			);
		},
	},
};
</script>

<style>
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}
</style>
