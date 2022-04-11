<!--  -->

<template>
<div class="marquee-50-50">

	<div class="left">
		<h1 class="title">Netlify Graph</h1>
		<p class="subhead">A faster way to develop with APIs</p>
		<div class="ctas">
			<nuxt-link to="/">
				<btn>Learn More</btn>
			</nuxt-link>
		</div>
	</div>

	<div class="right">
		<img src="graphql-playground.png" alt="Screenshot of GraphQL playground"/>
	</div>

</div>


</template>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<script>
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
	background: linear-gradient(176deg,#151a1e 0,#061475 90%);
	color: white;
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
