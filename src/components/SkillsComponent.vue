<template>
	<section id="skills">
		<h2 class="skills-title">Conhecimentos</h2>
		<div class="skills-divider"></div>
		<div class="skills-tags">
			<TagComponent>
				<img src="@/assets/icon-html5.png" alt="Logo html5" />
				<p>HTML5</p>
			</TagComponent>
			<TagComponent>
				<img src="@/assets/icon-css3.png" alt="Logo css3" />
				<p>CSS3</p>
			</TagComponent>
			<TagComponent>
				<img src="@/assets/icon-javascript.png" alt="Logo javascript" />
				<p>JavaScript</p>
			</TagComponent>
			<TagComponent>
				<img src="@/assets/icon-vue-js.png" alt="Logo vue.js" />
				<p>Vue.JS</p>
			</TagComponent>
			<TagComponent>
				<img src="@/assets/icon-react.png" alt="Logo react js" />
				<p>React JS</p>
			</TagComponent>
			<TagComponent>
				<img src="@/assets/icon-node-js.png" alt="Logo node js" />
				<p>Node JS</p>
			</TagComponent>
			<TagComponent>
				<img src="@/assets/icon-typescript.png" alt="Logo typescript" />
				<p>TypeScript</p>
			</TagComponent>
			<TagComponent>
				<img src="@/assets/icon-git.png" alt="Logo git" />
				<p>Git</p>
			</TagComponent>
			<TagComponent>
				<img src="@/assets/icon-github.png" alt="Logo github" />
				<p>GitHub</p>
			</TagComponent>
			<TagComponent>
				<img src="@/assets/icon-webpack.png" alt="Logo webpack" />
				<p>Webpack</p>
			</TagComponent>
		</div>
	</section>
</template>

<script>
	import TagComponent from "./TagComponent.vue";

	export default {
		name: "SkillsComponent",
		components: {
			TagComponent,
		},
	};
</script>

<style scoped>
	#skills {
		display: flex;
		align-items: center;
		padding: 120px 0;
	}

	.skills-title {
		font-family: "Ubuntu";
		font-style: normal;
		font-weight: 400;
		font-size: 36px;
		line-height: 110%;
		color: #e0ede7;
		padding-left: 108px;
	}

	.skills-divider {
		height: 396px;
		border-left: 2px solid #58625a;
		margin-left: 172px;
		margin-right: 108px;
	}

	.skills-tags {
		width: 100%;
		display: flex;
		flex-wrap: wrap;
		justify-content: center;
		align-content: center;
		gap: 36px;
	}
</style>
