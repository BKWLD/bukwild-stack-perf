<script setup>
import LayoutHeader from './components/layout/header.vue'
import MarqueeSplit from './components/marquee-50-50.vue'
import LogoGarden from './components/logo-garden.vue'
import MarqueeBlue from './components/marquee-blue.vue'
import LayoutFooter from './components/layout/footer.vue'

</script>

<template>

	<div id="app" class="page">
		<layout-header />

    <main id="main">

      <marquee-split />

      <logo-garden />

      <marquee-blue />

      <layout-footer />

    </main>

	</div>

</template>

<style>
.page {
	font-family: 'Arimo', Arial, sans-serif;

	/* Layout */
	--gutter: 60px;
	--gutter-mobile: 20px;
	--max-w-small: calc(750px + var(--gutter) * 2);
	--max-w-medium: calc(1060px + var(--gutter) * 2);
	--max-w: calc(1280px + var(--gutter) * 2);
	--max-w-wide: calc(1440px);
	--max-w-full: calc(2560px);

	/* Breakpoints */
	--desktop: 1440px;
	--tablet: 768px;
	--mobile: 500px;

	/* Colors */
	--blue: #2250F4;
	--light-grey: #f2f5f8;
}

/* Resets */
body {
  margin: 0;
}

a {
  color: black;
  text-decoration: none;
}

img {
  max-width: 100%;
}

</style>
