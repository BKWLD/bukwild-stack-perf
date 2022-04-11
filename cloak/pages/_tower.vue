<!-- Standard Block renderer -->

<template lang='pug'>

.tower

	//- GTM container with GA

	marquee-50-50

	logo-garden

	marquee-blue



</template>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<script lang='coffee'>
import pageMixin from '@bkwld/cloak/mixins/page'

export default
	name: 'Tower'

	mixins: [ pageMixin ]

	head: ->
		title: 'Netlify: Develop & deploy the best web experiences'

		# <link rel="preconnect" href="https://fonts.googleapis.com">
		# <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
		# <link href="https://fonts.googleapis.com/css2?family=Arimo:wght@700&display=swap" rel="stylesheet">

		link: [
			{
				rel: 'preconnect'
				href: 'https://fonts.googleapis.com'
			}
			{
				rel: 'preconnect'
				href: 'https://fonts.gstatic.com'
				crossorigin: true
			}
			{
				rel: 'stylesheet'
				href: 'https://fonts.googleapis.com/css2?family=Arimo:wght@400;500;700&display=swap'
			}
		]


	# Get Tower data
	asyncData: ({ app, params, payload }) ->

		page = {}

		# Get data
		return app.$notFound() unless page

		# Set data
		return { page }

</script>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<style lang='stylus' scoped>

</style>
