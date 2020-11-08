<script lang="ts">
	import Router from "svelte-spa-router";
	import routes from "./routes";

	import Navbar from "./components/Navbar.svelte";
	import Footer from "./components/Footer.svelte";
</script>

<main id="mainpanel" class="is-widescreen">
	<section id="mainpanel" class="hero is-dark is-fullheight">
		<Navbar />
		<Router {routes}/>
		<Footer />
	</section>
</main>

<style lang="scss" global>
	@charset "utf-8";

	// Import a Google Font
	@import url('https://fonts.googleapis.com/css?family=Nunito:400,700');

	// Set your brand colors
	$purple: #8A4D76;
	$pink: #FA7C91;
	$brown: #757763;
	$beige-light: #D0D1CD;
	$beige-lighter: #EFF0EB;

	// Update Bulma's global variables
	$family-sans-serif: "Nunito", sans-serif;
	$grey-dark: $brown;
	$grey-light: $beige-light;
	$primary: $purple;
	$link: $pink;
	$widescreen-enabled: true;
	$fullhd-enabled: true;


	// Import only what you need from Bulma
	@import "../node_modules/bulma/sass/utilities/_all.sass";
	@import "../node_modules/bulma/sass/base/_all.sass";
	@import "../node_modules/bulma/sass/elements/_all.sass";
	@import "../node_modules/bulma/sass/form/_all.sass";
	@import "../node_modules/bulma/sass/components/_all.sass";
	@import "../node_modules/bulma/sass/grid/_all.sass";
	@import "../node_modules/bulma/sass/helpers/_all.sass";
	@import "../node_modules/bulma/sass/layout/_all.sass";

	#mainpanel {
    background: linear-gradient( rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5) ), url('https://unsplash.it/1200/900?random') no-repeat center center fixed;
    background-size: cover;
  }
</style>
