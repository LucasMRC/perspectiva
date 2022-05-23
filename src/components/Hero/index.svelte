<script lang="ts">
    import Navbar from "./Navbar/index.svelte";
    import Title from "./Title.svelte";
</script>

<div class="hero">
    <Navbar />
    <Title />
</div>

<style>

    div.hero {
        background: no-repeat url(/turtle-background.jpg) center / cover;
        width: 100%;
        height: 100vh;
    }

</style>