<template>
	<section id="hero">
		<div class="hero-left">
			<h2>Olá, eu sou</h2>
			<h1>Pedro Gutierres</h1>
			<div class="phrases">
				<span class="phrase-1">Desenvolvimento Web</span>
				<span class="phrase-2">Front end</span>
				<span class="phrase-3">"A simplicidade é o último grau da sofisticação"<br />Da Vinci</span>
			</div>
		</div>
		<div class="hero-right">
			<span>Seja bem-vindo,</span>
			<div class="hero-description">
				<p class="hero-considerations">
					Um desenvolvedor frontend apaixonado pela criação de interfaces e experiência do usuário.
				</p>
				<ButtonComponent class="btn-hero" :link="linkedin">
					<img src="@/assets/linkedin-icon.png" alt="Logo linkedIn" />
					<p>LinkedIn</p>
				</ButtonComponent>
			</div>
		</div>
	</section>
</template>

<script>
	import ButtonComponent from "./ButtonComponent.vue";

	export default {
		name: "HeroComponent",
		components: {
			ButtonComponent,
		},
		data() {
			return {
				linkedin: "https://www.linkedin.com/in/pedrogabrielgutierres/",
			};
		},
	};
</script>

<style scoped>
	h1 {
		width: 100%;
		text-align: center;
		font-family: "Ubuntu";
		font-style: normal;
		font-weight: 500;
		font-size: 72px;
		line-height: 120%;
		background: linear-gradient(251.7deg, #3fb984 0%, #e0ede7 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
		background-clip: text;
		font-size: 72px;
	}

	h2 {
		font-family: "Ubuntu";
		font-style: normal;
		font-weight: 400;
		font-size: 36px;
		line-height: 110%;
		color: #a8b2b2;
	}

	span,
	p {
		font-family: "Mukta";
		font-style: normal;
		font-weight: 400;
		color: #a8b2b2;
	}

	#hero {
		display: flex;
		justify-content: space-between;
		align-content: center;
		padding: 216px 0;
	}

	.hero-left > h2 {
		margin-bottom: 20px;
	}

	.hero-left > h1 {
		margin-bottom: 32px;
		margin-left: 18px;
	}

	.phrases {
		display: flex;
		flex-direction: column;
	}

	.phrases span {
		font-size: 18px;
		line-height: 140%;
	}

	.phrase-1 {
		margin: 0 0 16px 72px;
	}

	.phrase-2 {
		margin: 0 0 16px 0;
	}

	.phrase-3 {
		margin: 0 0 0 110px;
	}

	.hero-right {
		width: 45%;
	}

	.hero-right > span {
		display: block;
		margin-bottom: 32px;
		font-size: 18px;
		line-height: 140%;
	}

	.hero-right > div {
		margin-left: 16px;
	}

	.hero-considerations {
		margin-bottom: 24px;
		font-size: 24px;
		line-height: 140%;
	}
</style>
