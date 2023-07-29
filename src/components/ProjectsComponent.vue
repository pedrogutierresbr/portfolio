<template>
	<section id="projects">
		<div class="prjects-left">
			<h2 class="projects-title">Projetos</h2>
			<div class="phrases">
				<p class="phrase-1">Inspiração</p>
				<p class="phrase-2">Criação</p>
				<p class="phrase-3">Execução</p>
			</div>
		</div>

		<div class="projects-divider"></div>

		<div class="projects-right">
			<div class="project project-1">
				<img src="@/assets/projects-dark.png" alt="imagem representativa logo do projeto" />
				<div>
					<h3 class="project-title">Portfólio</h3>
					<p class="project-description">
						Site portfólio, criado utilizando conceitos de design minimalista e com o uso da tecnologia Vue.JS.
					</p>
					<a href="/"><p class="project-link">Lorem ipsum dolor sit amet, consectetur</p></a>
				</div>
			</div>

			<div class="project project-2">
				<div>
					<h3 class="project-title">Guti Store</h3>
					<p class="project-description">
						Projeto criado para simular a experiência de um pequeno e-commerce utilizando a tecnologia Vue.js
					</p>
					<a href="/"><p class="project-link">Lorem ipsum dolor sit amet, consectetur</p></a>
				</div>
				<img src="@/assets/projects-white.png" alt="imagem representativa logo do projeto" />
			</div>

			<div class="project project-3">
				<img src="@/assets/projects-white.png" alt="imagem representativa logo do projeto" />
				<div>
					<h3 class="project-title">Microfrontend com Webpack</h3>
					<p class="project-description">
						Projeto criado com a ferramenta Webpack. Utilizando a feature Module Federation para simular uma arquitetura de
						micro-frontend.
					</p>
					<a href="/"><p class="project-link">Lorem ipsum dolor sit amet, consectetur</p></a>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
	export default {
		name: "ProjectsComponent",
	};
</script>

<style>
	h3 {
		margin: 0;
	}

	#projects {
		display: flex;
		padding: 120px 0;
	}

	.prjects-left {
		padding-left: 108px;
		height: 100%;
		display: flex;
		flex-direction: column;
		align-items: flex-start;
	}

	.projects-title {
		font-family: "Ubuntu";
		font-style: normal;
		font-weight: 400;
		font-size: 36px;
		line-height: 110%;
		color: #e0ede7;
	}

	.phrases {
		margin-top: 52px;
		color: #a8b2b2;
		font-family: "Mukta";
		font-style: normal;
		font-weight: 400;
		display: flex;
	}

	.phrases p {
		font-size: 18px;
		line-height: 140%;
	}

	.phrase-1 {
		width: 100%;
	}

	.phrase-2 {
		margin: 40px 0 0 36px;
	}

	.phrase-3 {
		margin: 65px 0 0 36px;
	}

	.projects-divider {
		border-left: 2px solid #58625a;
		margin-left: 150px;
		margin-right: 108px;
	}

	.projects-right {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: flex-start;
		margin-top: 58px;
	}

	.project {
		display: flex;
	}

	.project img {
		width: 180px;
		height: 180px;
	}

	.project-1 img,
	.project-3 img {
		margin-right: 36px;
	}

	.project-2 {
		margin: 144px 0px;
	}

	.project-2 div {
		margin-right: 26px;
	}

	.project-title {
		font-family: "Ubuntu";
		font-size: 24px;
		font-weight: 400;
		line-height: 110%;
		color: #e0ede7;
		margin-bottom: 24px;
	}

	.project-description,
	.project-link {
		font-family: "Mukta";
		font-size: 18px;
		font-weight: 400;
		line-height: 140%;
	}

	.project-description {
		width: 320px;
		color: #a8b2b2;
		margin-bottom: 24px;
	}

	.project-link {
		background: linear-gradient(251.7deg, #3fb984 0%, #e0ede7 100%);
		-webkit-background-clip: text;
		background-clip: text;
		color: transparent;
	}
</style>
