<!-- Spacer block -->

<template lang='pug'>

section.spacer(:class='classes')

</template>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<script lang='coffee'>
export default

	props: block: Object

</script>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<style lang='stylus' scoped>

.spacer
	&.height-s
		fluid-space height, 's'
	&.height-m
		fluid-space height, 'm'
	&.height-l
		fluid-space height, 'l'
	&.height-xl
		fluid-space height, 'xl'

</style>
