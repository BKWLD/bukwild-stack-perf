<!--  -->

<template>
	<header>
		<div class="left">
			<a href="/">
				<img src="/netlify-logo.svg" alt="Netlify Logo" class="logo"/>
			</a>
		</div>

		<div class="center">
			<nuxt-link to="/">Platform</nuxt-link>
			<nuxt-link to="/">Pricing</nuxt-link>
			<nuxt-link to="/">Enterprise</nuxt-link>
			<nuxt-link to="/">Customers</nuxt-link>
			<nuxt-link to="/">Blog</nuxt-link>
			<nuxt-link to="/">Docs</nuxt-link>
		</div>

		<div class="right">
			<nuxt-link to="/">
				<btn>Sign up</btn>
			</nuxt-link>
		</div>

	</header>



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

header {
	display: flex;
	flex-direction: row;
	flex-wrap: nowrap;

	padding: 0 var(--gutter);
	margin: 40px auto;
	max-width: var(--max-w-wide);
	font-weight: 700;
}

.logo {
	width: 100px;
}

.center > * {
	position: relative;
	top: 6px;
	padding-left: 22px;
	font-size: 15px;
}

.right {
	flex-grow: 1;
	display: flex;
	justify-content: flex-end;
}

</style>
