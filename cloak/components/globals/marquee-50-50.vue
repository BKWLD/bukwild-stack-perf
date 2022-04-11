<!--  -->

<template>
<div class="marquee-50-50">

	<div class="left">
		<h1 class="title">Build the future of the web</h1>
		<p class="subhead">Netlify unites an entire ecosystem of modern tools and services into a single, simple workflow for building high performance sites and apps.</p>
		<div class="ctas">
			<nuxt-link to="/get-started">
				<btn>Get started for free</btn>
			</nuxt-link>
			<nuxt-link to="/get-started">Questions? Talk to an expert
			</nuxt-link>
		</div>
	</div>

	<div class="right">
		<img src="/marquee-image.avif" alt="Screenshot of code editor and an ecommerce website"/>
	</div>

</div>


</template>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<script lang='coffee'>
# export default
# 	components:
# 	props: []
# 	data: ->
# 	computed:
# 	watch:
# 	methods:
</script>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<style scoped>

.marquee-50-50 {
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	align-items: center;
	margin: 0 auto;
	padding: 0 var(--gutter);
	max-width: var(--max-w-wide);
}

.left, .right {
	width: 50%;
	padding: 20px 0;
}

@media (max-width: 768px) {
	.left, .right {
		width: 100%;
	}
}

.title {
	font-size: 60px;
	letter-spacing: -2px;
	font-weight: 700
}

.subhead {
	font-size: 24px;
	line-height: 1.3;
	font-weight: 500;
}

.ctas {
	margin-top: 40px;
	font-weight: 700;
}

.ctas > * {
	margin-right: 20px;
}

</style>
