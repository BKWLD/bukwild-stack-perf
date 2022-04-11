<!-- General layout -->

<template>

<div class="default-layout">
	<a class="skip-content" href="#main">Skip to main content</a>

	<layout-header />

	<main id="main">
		<nuxt class="page"></nuxt>

		<layout-footer />

	</main>

</div>

</template>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<script lang='coffee'>
export default
	name: 'DefaultLayout'

</script>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<style lang='stylus' scoped>

// Prevent mega-wide pages
.default-layout
	max-width max-w-full
	margin-h auto
	width 100%
	overflow hidden

// On short pages, pin the footer to the bottom of the page
main
	min-height 100vh
	display flex
	flex-direction column
.page
	flex-grow 1

.skip-content
	position absolute
	left -1000px
	+tablet-up()
		top (header-h + spacing-s)
	+tablet-down()
		top (header-h-mobile + spacing-s-min)
	z-index header-z // stacked below nav but above page content

	&:focus
		fluid left, gutter, gutter-mobile
		outline none

</style>

<style scoped>
.default-layout {
	font-family: 'Arimo', Arial, sans-serif;

	/* Layout */
	--gutter: 60px;
	--gutter-mobile: 20px;
	--max-w-small: calc(750px + gutter * 2);
	--max-w-medium: calc(1060px + gutter * 2);
	--max-w: calc(1280px + gutter * 2);
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
</style>
