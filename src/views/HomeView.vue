<template>
	<div>
		<HeroComponent />
		<ProjectsComponent />
		<ExperienceComponent />
		<AboutComponent />
		<SkillsComponent />
		<ContactComponent />
	</div>
</template>

<script>
	import HeroComponent from "@/components/HeroComponent.vue";
	import ProjectsComponent from "@/components/ProjectsComponent.vue";
	import ExperienceComponent from "@/components/ExperienceComponent.vue";
	import AboutComponent from "@/components/AboutComponent.vue";
	import SkillsComponent from "@/components/SkillsComponent.vue";
	import ContactComponent from "@/components/ContactComponent.vue";

	export default {
		name: "HomeView",
		components: {
			HeroComponent,
			ProjectsComponent,
			ExperienceComponent,
			AboutComponent,
			SkillsComponent,
			ContactComponent,
		},
	};
</script>

<style scoped></style>
