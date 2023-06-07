<template>
	<footer>
		<router-link to="/">
			<img src="@/assets/main-icon.png" alt="Logo" @click="rollUp()" />
		</router-link>
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
		methods: {
			getYear() {
				const date = new Date().getFullYear();
				this.year = date;
			},
			rollUp() {
				window.scrollTo({ top: 0, behavior: "smooth" });
			},
		},
		created() {
			this.getYear();
		},
	};
</script>

<style scoped>
	footer {
		width: 100%;
		padding: 15px;
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
		font-weight: 400;
		margin-top: 10px;
		color: #e0ede7;
	}
</style>
