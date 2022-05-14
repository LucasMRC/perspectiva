<script lang="ts">
    import ArticleOne from './articleOne.svelte';
    import ArticleTwo from './articleTwo.svelte';
</script>

<main>
    <ArticleOne />
    <hr />
    <!-- <ArticleTwo /> -->
</main>

<style>

    main {
        width: 100%;
        padding: 5rem 3rem;
        min-height: 100vh;
        box-sizing: border-box;
    }

    @media screen and (min-width: 480px) {
        main {
            width: 65%;
            padding: 5rem 0 5rem 12rem;
        }
    }

</style>