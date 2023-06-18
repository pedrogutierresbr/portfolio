<template>
	<section id="contact">
		<h2>Contato</h2>
		<p>Pronto para iniciar um projeto? Entre em contato e vamos criar algo incrível juntos.</p>
		<div class="social-networks">
			<ButtonComponent :link="links.intagram">
				<img src="@/assets/instagram-icon.png" alt="Logo instagram" />
				<p>Instagram</p>
			</ButtonComponent>
			<ButtonComponent :link="links.linkedin">
				<img src="@/assets/linkedin-icon.png" alt="Logo linkedIn" />
				<p>LinkedIn</p>
			</ButtonComponent>
			<ButtonComponent :link="links.whatsapp">
				<img src="@/assets/whatsapp-icon.png" alt="Logo whatsapp" />
				<p>WhatsApp</p>
			</ButtonComponent>
		</div>
	</section>
</template>

<script>
	import ButtonComponent from "./ButtonComponent.vue";
	export default {
		name: "ContactComponent",
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
		components: {
			ButtonComponent,
		},
	};
</script>

<style scoped>
	#contact {
		width: 100%;
		padding: 110px 0 220px;
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	h2 {
		color: #e0ede7;
		font-size: 36px;
		line-height: 110%;
		text-align: center;
		margin-bottom: 64px;
		font-weight: 400;
	}

	p {
		color: #c4d0cd;
		font-size: 18px;
		line-height: 140%;
		text-align: center;
		margin-bottom: 96px;
	}

	.social-networks {
		width: 65.75%;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
</style>
