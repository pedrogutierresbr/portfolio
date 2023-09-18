<template>
	<div id="experience">
		<h2>Experiência</h2>
		<div class="experience-body">
			<div class="experience-companies">
				<p class="experience-company active">Risk Adviser</p>
				<p class="experience-company">Cuponomia</p>
				<p class="experience-company">Feelancer</p>
			</div>

			<div class="experience-contents">
				<div class="experience-content">
					<div class="experience-content-header">
						<p class="experience-content-header-title">Risk Adviser</p>
						<p class="experience-content-header-period">Jun 2023 - atualmente</p>
					</div>
					<p class="experience-content-ocupation">Desenvolvedor Web Frontend</p>
					<p class="experience-content-description">
						Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa accusamus nulla fugiat assumenda maiores dignissimos,
						eveniet omnis id necessitatibus harum inventore? Quaerat voluptates a reiciendis quis ratione rerum voluptatem
						fugit. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa accusamus nulla fugiat assumenda maiores
						dignissimos, eveniet omnis id necessitatibus harum inventore? Quaerat voluptates a reiciendis quis ratione rerum
						voluptatem fugit.
					</p>
				</div>

				<div class="experience-content hide">
					<div class="experience-content-header">
						<p class="experience-content-header-title">Cuponomia</p>
						<p class="experience-content-header-period">Ago 2021 - Fev 2023</p>
					</div>
					<p class="experience-content-ocupation">Desenvolvedor Web Frontend</p>
					<p class="experience-content-description">
						Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa accusamus nulla fugiat assumenda maiores dignissimos,
						eveniet omnis id necessitatibus harum inventore? Quaerat voluptates a reiciendis quis ratione rerum voluptatem
						fugit. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa accusamus nulla fugiat assumenda maiores
						dignissimos, eveniet omnis id necessitatibus harum inventore? Quaerat voluptates a reiciendis quis ratione rerum
						voluptatem fugit.
					</p>
				</div>

				<div class="experience-content hide">
					<div class="experience-content-header">
						<p class="experience-content-header-title">Freelancer</p>
						<p class="experience-content-header-period">Ago 2021 - atualmente</p>
					</div>
					<p class="experience-content-ocupation">Desenvolvedor Web Frontend</p>
					<p class="experience-content-description">
						Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa accusamus nulla fugiat assumenda maiores dignissimos,
						eveniet omnis id necessitatibus harum inventore? Quaerat voluptates a reiciendis quis ratione rerum voluptatem
						fugit. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsa accusamus nulla fugiat assumenda maiores
						dignissimos, eveniet omnis id necessitatibus harum inventore? Quaerat voluptates a reiciendis quis ratione rerum
						voluptatem fugit.
					</p>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: "ExperienceComponent",
	};
</script>

<style scoped lang="scss">
	#experience {
		padding: 120px 80px 120px 108px;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: flex-start;
	}

	.hide {
		display: none !important;
	}

	h2 {
		color: #e0ede7;
		font-size: 36px;
		line-height: 110%;
		text-align: center;
		margin-bottom: 64px;
		font-weight: 400;
	}

	.active {
		color: #3fb984 !important;
	}

	.experience {
		&-body {
			display: flex;
			justify-content: flex-start;
			align-items: center;
			gap: 108px;
		}

		&-companies {
			display: flex;
			flex-direction: column;
			justify-content: flex-start;
			align-items: center;
			padding: 70px 35px;
			color: white;
			min-width: 220px;
			height: 340px;
			border-radius: 32px;
			position: relative;
			background: transparent;
			border: none;

			&::before {
				content: "";
				position: absolute;
				inset: 0;
				padding: 2px;
				border-radius: 32px;
				background: linear-gradient(45deg, #e0ede7 0%, #3fb984 100%);
				mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
				mask-composite: exclude;
			}
		}

		&-company {
			font-size: 24px;
			line-height: 110%;
			font-weight: 400;
			color: #e0ede7;
			margin-bottom: 40px;
			cursor: pointer;
			z-index: 1000;
		}

		&-content {
			display: flex;
			flex-direction: column;
			align-items: flex-start;

			&-header {
				width: 100%;
				display: flex;
				justify-content: space-between;
				margin-bottom: 40px;

				&-title {
					font-size: 24px;
					font-weight: 400;
					line-height: 110%;
					color: #e0ede7;
				}

				&-period {
					font-family: Mukta, Helvetica, sans-serif;
					font-size: 16px;
					font-weight: 400;
					line-height: 150%;
					color: #a8b2b2;
				}
			}

			&-ocupation,
			&-description {
				font-family: Mukta, Helvetica, sans-serif;
				font-size: 18px;
				font-weight: 400;
				line-height: 150%;
				color: #a8b2b2;
			}

			&-ocupation{
				margin-bottom: 40px;
			}
		}
	}
</style>
