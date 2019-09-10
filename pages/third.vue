<template lang="pug">
	section.container.dignity(style=" display: flex; justify-content: center; flex-direction: column; height: 400px;")
		h1.md-display-1 Volcanic Measurements
		img(src="biohazard.svg" width="175px")
		h1.headline(style="margin-bottom: 0px;")
			| A Not Unexpected Tutorial
		h3.subheading(style="margin: 0px;")
			| Vue Material, Square One Again
		md-button.md-accent.md-raised(style="margin-top: 15px;" to="/fourth")
			md-icon waves
			| &nbsp; Nuxt in a Tuxt
</template>

<style>
.container {
	min-height: 100vh;
	display: flex;
	justify-content: center;
	align-items: center;
	text-align: center;
	flex-direction: column;
	line-height: 2.0;
	min-height: 75vh
}

.title {
	font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
	display: block;
	font-weight: 300;
	font-size: 100px;
	color: #35495e;
	letter-spacing: 1px;
}

.subtitle {
	font-weight: 300;
	font-size: 42px;
	color: #526488;
	word-spacing: 5px;
	padding-bottom: 15px;
}

.links {
	padding-top: 15px;
}
</style>
