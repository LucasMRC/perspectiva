<script lang="ts">
	import Main from "./lib/Main/index.svelte"
	import Hero from "./lib/Hero/index.svelte";
	import Footer from "./lib/Footer/index.svelte";
</script>

<div class="body">
	<Hero/>
	<Main />
	<Footer />
</div>

<style>
	div.body {
		position: relative;
		scroll-behavior: smooth;
	}
</style>
