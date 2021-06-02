<template>
	<div id="app">
		<News :apiKey="apiKey" />
	</div>
</template>

<script>
	import News from "./components/News.vue";

	export default {
		name: "App",
		data: () => {
			return {
				apiKey: "51fe3254e2a44244b5196a7c986c5954",
			};
		},
		components: {
			News,
		},
	};
</script>

<style lang="scss">
	@import url("https://use.fontawesome.com/releases/v5.7.2/css/all.css");

	body {
		margin: 0;
		padding: 0;
		width: 100%;
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: center;
		background: linear-gradient(to bottom, #80a248, #198b4d);
	}
	#app {
		font-family: Arial, Helvetica, sans-serif;
		font-size: 1rem;
		color: #333;
		width: 100%;
		height: 100%;
		background-color: #fff;
		/*
    border: 2px solid #222;
    border-radius: 20px;
    box-shadow: 5px 10px 18px #222;
    */
		overflow-y: scroll;
		overflow-x: hidden;
	}
	::-webkit-scrollbar {
		display: none;
	}
</style>
