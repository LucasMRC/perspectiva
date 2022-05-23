<script lang="ts">
    import ArticleOne from './articleOne.svelte';
    import ArticleTwo from './articleTwo.svelte';
    import { article } from '../../utils/stores';

    let currentArticle: number;

    article.subscribe(newArticle => {
        currentArticle = newArticle;
    });

</script>

<main>

    <!-- svelte-ignore component-name-lowercase -->
    <article
        id="article"
    >
        {#if currentArticle === 1}
            <ArticleOne />
        {/if}
        {#if currentArticle === 2}
            <ArticleTwo />
        {/if}
        <!-- {#if article === 3}
            <ArticleThree />
        {/if} -->
    </article>
</main>