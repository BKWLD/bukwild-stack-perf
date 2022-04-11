<template>
  <div class="tower">

    <Layout-Header />

    <main id="main">

      <Marquee-50-50 />

      <Logo-Garden />

      <Marquee-Blue />

      <Layout-Footer />

    </main>

  </div>


</template>

<script>
export default {
  name: 'IndexPage',

	head: () => { return {
		title: 'Netlify: Develop & deploy the best web experiences',

    // # <link rel="preconnect" href="https://fonts.googleapis.com">
    // # <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    // # <link href="https://fonts.googleapis.com/css2?family=Arimo:wght@700&display=swap" rel="stylesheet">
		link: [
			{
				rel: 'preconnect',
				href: 'https://fonts.googleapis.com'
			},
			{
				rel: 'preconnect',
				href: 'https://fonts.gstatic.com',
				crossorigin: true
			},
			{
				rel: 'stylesheet',
				href: 'https://fonts.googleapis.com/css2?family=Arimo:wght@400;500;700&display=swap'
			}
		]
  }}

}
</script>

<style>
.tower {
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
