<template>
	<div>
		<button class="gradient-border">
			<slot></slot>
		</button>
	</div>
</template>

<script>
	export default {
		name: "TagComponent",
	};
</script>

<style scoped>
	.gradient-border {
		cursor: pointer;
		font-family: Mukta, Helvetica, sans-serif;
		display: flex;
		justify-content: center;
		align-items: center;
		padding: 10px 20px;
		color: white;
		width: 180px;
		height: 72px;
		border-radius: 8px;
		position: relative;
		background: transparent;
		border: none;
	}
	.gradient-border::before {
		content: "";
		position: absolute;
		inset: 0;
		padding: 2px;
		border-radius: 8px;
		background: linear-gradient(45deg, #e0ede7 0%, #3fb984 100%);
		mask: linear-gradient(#fff 0 0) content-box, linear-gradient(#fff 0 0);
		mask-composite: exclude;
	}

	.gradient-border img {
		width: 32px;
		height: 32px;
		margin-right: 8px;
	}

	.gradient-border p {
		font-size: 16px;
		line-height: 150%;
		margin: 0;

		background: linear-gradient(45deg, #e0ede7 0%, #3fb984 100%);
		background-clip: text;
		-webkit-text-fill-color: transparent;
		color: #0d1215;
	}
</style>
