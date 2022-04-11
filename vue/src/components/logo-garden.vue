<script setup>
import LogoGardenLogos from './logo-garden-logos.vue'
</script>

<template>
	<div class="logo-garden">
		<h2 class="title">
			Millions of developers and businesses trust Netlify.
			<smart-link to="/see-more">See More</smart-link>
		</h2>

		<logo-garden-logos/>
	</div>
</template>


<style scoped>
.logo-garden {
	margin: 0 auto;
	padding: 80px var(--gutter);
	max-width: var(--max-w-wide);
	background-color: var(--light-grey);
}

.title {
	text-align: center;
	text-transform: uppercase;
	font-size: 18px;
	font-weight: 700;
	letter-spacing: 0.4px;
}

/* .unilever {
}
.tripactions */

</style>
