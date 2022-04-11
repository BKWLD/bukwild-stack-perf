<!--  -->

<script setup>
import Btn from '../btn.vue'

</script>


<template>
	<header>
		<div class="left">
			<a href="/">
				<img src="../../../assets/netlify-logo.svg" alt="Netlify Logo" class="logo"/>
			</a>
		</div>

		<div class="center">
			<a href="/">Platform</a>
			<a href="/">Pricing</a>
			<a href="/">Enterprise</a>
			<a href="/">Customers</a>
			<a href="/">Blog</a>
			<a href="/">Docs</a>
		</div>

		<div class="right">
			<a href="/">
				<Btn>Sign up</Btn>
			</a>
		</div>

	</header>



</template>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->


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
