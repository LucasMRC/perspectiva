<script lang="ts">
    import ArticleOne from './articles/articleOne.svelte';
    import ArticleTwo from './articles/articleTwo.svelte';
	import { article } from '@utils/stores';

    let currentArticle: number;
    export let language: string;

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
            <ArticleOne
                language={language}
            />
        {:else if currentArticle === 2}
            <ArticleTwo
                language={language}
            />
        {/if}
    </article>
</main>