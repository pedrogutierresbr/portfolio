<template>
	<header>
		<nav>
			<router-link to="#about">Sobre</router-link>
			<router-link to="#experience">Experiência</router-link>
			<router-link to="/">
				<img src="@/assets/main-icon.png" alt="Logo" @click="rollUp" />
			</router-link>
			<router-link to="#projects">Trabalhos</router-link>
			<router-link to="#contact">Contato</router-link>
		</nav>
	</header>
</template>

<script>
	export default {
		name: "HeaderComponent",
		methods: {
			rollUp() {
				window.scrollTo({ top: 0, behavior: "smooth" });
			},
		},
	};
</script>

<style scoped>
	header {
		position: fixed;
		width: 100%;
		height: 110px;

		background: linear-gradient(
			180deg,
			rgba(255, 255, 255, 0.1) 0%,
			rgba(255, 255, 255, 0.3) 100%,
			rgba(255, 255, 255, 0.3) 100%
		);
		border-bottom: 1px solid rgba(255, 255, 255, 0.2);
		box-shadow: inset 10px 10px 10px rgba(0, 0, 0, 0.1);
		backdrop-filter: blur(10px);
		z-index: 10;
	}

	nav {
		width: 1260px;
		height: 100%;
		margin: 0 auto;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	a {
		line-height: 140%;
		font-size: 18px;
		font-weight: 400;
		color: #e0ede7;
	}
</style>
