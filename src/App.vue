<template>
	<div id="app">
		<HeaderComponent />
		<main id="main">
			<router-view />
		</main>
		<FooterComponent />
	</div>
</template>

<script>
	import HeaderComponent from "@/components/HeaderComponent.vue";
	import FooterComponent from "@/components/FooterComponent.vue";

	export default {
		name: "App",
		components: {
			HeaderComponent,
			FooterComponent,
		},
	};
</script>

<style>
	* {
		box-sizing: border-box;
	}

	body,
	ul,
	li,
	h1,
	h2,
	p {
		margin: 0;
		padding: 0;
	}

	h1,
	h2,
	h3 {
		font-family: Ubuntu, Helvetica, sans-serif;
	}

	p,
	a {
		font-family: Mukta, Helvetica, sans-serif;
	}

	ul {
		list-style: none;
	}

	body {
		background: #0d1215;
	}

	a {
		color: #345;
		text-decoration: none;
	}

	img {
		max-width: 100%;
		display: block;
	}

	label {
		margin-bottom: 5px;
	}

	input,
	textarea {
		border-radius: 4px;
		border: 1px solid white;
		padding: 15px;
		box-shadow: 0 4px 8px rgba(30, 60, 90, 0.1);
		transition: all 0.3s;
		font-size: 1rem;
		font-family: Arial, Helvetica, sans-serif;
		margin-bottom: 15px;
	}

	input:hover,
	input:focus,
	textarea:hover,
	textarea:focus {
		outline: none;
		box-shadow: 0 6px 12px rgba(30, 60, 90, 0.2);
		border-color: #3fb984;
	}

	#app {
		display: flex;
		min-height: 100vh;
		flex-direction: column;
	}

	#main {
		flex: 1;
	}
</style>
