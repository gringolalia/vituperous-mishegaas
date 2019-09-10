<template lang="pug">
	.page-container
		md-app(md-mode='reveal')
			md-app-toolbar.md-primary

				md-button.md-icon-button(@click='menuVisible = !menuVisible')
					md-icon menu

				span.md-title(style="flex: 1")
					i.fa.fa-gears.fa-2x
					| &nbsp; Engenho Novo LLC

				md-toolbar-section-end
					md-button.md-icon-button(to="/" exact)
						md-icon more_vert
					md-button.md-icon-button(to="/second" exact)
						md-icon all_inclusive
					md-button.md-icon-button(to="fourth" exact)
						md-icon tv
					md-button.md-icon-button(to="third" exact)
						md-icon rowing

			md-app-drawer(:md-active.sync='menuVisible')
				md-toolbar.md-accent(md-elevation='6' style="font-size: 1.25em; text-align: right")
					i.fa.fa-anchor.fa-lg
					| &nbsp; &nbsp; Navegar é Preciso?

				md-list(@click="menuVisible = false")

					md-list-item(to="/" exact)
						md-icon fastfood

						span.md-list-item-text In and Out Urge

					md-list-item(to="/first" exact)
						md-icon transform

						span.md-list-item-text Voracious Underworld

					md-list-item(to="/second" exact)
						md-icon directions_boat

						span.md-list-item-text Velvet Underground

					md-list-item(to="/third" exact)
						md-icon directions_bike

						span.md-list-item-text Very Understated

					md-list-item(to="/fourth" exact)
						md-icon wb_sunny

						span.md-list-item-text Vituperous Mishegaas

					md-list-item(to="/fifth" exact)
						md-icon add_location

						span.md-list-item-text Vamoose Mister

			md-app-content
				nuxt
</template>

<script>
export default {
  name: 'Reveal',
  data: () => ({
    menuVisible: false
  })
}
</script>

<style lang="scss" scoped>
html {
	font-family: "News Cycle", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
	font-size: 16px;
	word-spacing: 1px;
	-ms-text-size-adjust: 100%;
	-webkit-text-size-adjust: 100%;
	-moz-osx-font-smoothing: grayscale;
	-webkit-font-smoothing: antialiased;
	box-sizing: border-box;
}

*, *:before, *:after {
	box-sizing: border-box;
	margin: 0;
}

  .md-toolbar + .md-toolbar {
    margin-top: 16px;
  }

</style>

</style>
