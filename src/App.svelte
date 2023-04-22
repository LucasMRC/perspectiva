<script lang="ts">
	import Main from "./components/Main/index.svelte"
	import Hero from "./components/Hero/index.svelte";
	import Footer from "./components/Footer/index.svelte";
	import { locale } from './utils/stores';

	const browserLanguage = (new Intl.NumberFormat()).resolvedOptions().locale.split('-')[0];

	if (browserLanguage === 'es') {
		locale.update(() => 'es');
	} else {
		locale.update(() => 'en');
	}
</script>

<div class="body">
	<Hero/>
	<Main language={browserLanguage || 'en'}/>
	<Footer />
</div>

<style>
	div.body {
		position: relative;
		scroll-behavior: smooth;
	}
</style>