<template>
	<footer>
		<img src="@/assets/main-icon.png" alt="Logo" />
		<p>Copyright &#169; {{ year }} Pedro Gutierres. Todos os direitos reservados</p>
	</footer>
</template>

<script>
	export default {
		name: "FooterComponent",
		data() {
			return {
				year: null,
			};
		},
	};
</script>

<style scoped>
	footer {
		padding: 15px 0;
		text-align: center;
		font-size: 1.2rem;
		color: #fff;
		position: relative;
		top: 135px;
		background: linear-gradient(180deg, rgba(255, 255, 255, 0.3) 0%, rgba(255, 255, 255, 0.1) 100%);
		border-top: 1px solid rgba(255, 255, 255, 0.2);
		box-shadow: inset 10px 10px 10px rgba(0, 0, 0, 0.1);
		backdrop-filter: blur(10px);
	}

	img {
		margin: 0 auto;
	}

	p {
		line-height: 140%;
		font-size: 18px;
		margin-top: 10px;
	}
</style>
