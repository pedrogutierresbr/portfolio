<template>
	<section id="about">
		<img class="image-developer" src="@/assets/pedro-gutierres-image.png" alt="Imagem de um desenvolvedor" />
		<div class="content">
			<h2>Quem é Pedro Gutierres ?</h2>
			<p>
				Desenvolvedor frontend atuando a mais de 2 anos na área. Possuo experiência em interfaces modernas e de
				alta qualidade, que proporcionem uma ótima experiência ao usuário e focando em performance e SEO para
				entregar interfaces de alto valor.
			</p>
			<p>
				Sempre a procura de novos desafios e disposto a agregar valor ao cliente/empresa. Segue abaixo minhas
				redes de contato, vamos criar algo fantástico juntos.
			</p>
			<div class="social-nets">
				<a :href="links.intagram" target="_blank">
					<img src="@/assets/instagram-icon.png" alt="logo intagram" />
				</a>
				<a :href="links.linkedin" target="_blank">
					<img src="@/assets/linkedin-icon.png" alt="logo linkedin" />
				</a>
				<a :href="links.whatsapp" target="_blank">
					<img src="@/assets/whatsapp-icon.png" alt="logo whatsapp" />
				</a>
			</div>
		</div>
	</section>
</template>

<script>
	export default {
		name: "AboutComponent",
		data() {
			return {
				links: {
					intagram: "https://www.instagram.com/pegutierres/",
					linkedin: "https://www.linkedin.com/in/pedrogabrielgutierres/",
					whatsapp:
						"https://api.whatsapp.com/send?phone=5512981890805&text=Olá!%20Tenho%20interesse%20em%20seus%20serviços%20relacionados%20a%20desenvolvimento%20de%20sites.",
				},
			};
		},
	};
</script>

<style scoped>
	#about {
		padding: 230px 0;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}

	.image-developer {
		margin-left: 50px;
	}

	.content {
		width: 44%;
		display: flex;
		flex-direction: column;
		align-items: flex-start;
	}

	.content h2 {
		font-family: "Ubuntu";
		font-style: normal;
		font-weight: 300;
		font-size: 48px;
		line-height: 110%;
		color: #e0ede7;
		margin-bottom: 40px;
	}

	.content p {
		width: 90%;
		font-family: "Mukta";
		font-style: normal;
		font-weight: 400;
		font-size: 18px;
		line-height: 140%;
		color: #c4d0cd;
	}

	.content p:first-of-type {
		margin-bottom: 12px;
	}

	.social-nets {
		width: 192px;
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin-top: 40px;
	}

	.social-nets a {
		width: 32px;
		height: 32px;
	}
</style>
