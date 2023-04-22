<script lang="ts">
    import ArticleOne from './articles/articleOne.svelte';
    import ArticleTwo from './articles/articleTwo.svelte';
	import { article } from '@utils/stores';

    let currentArticle: number;
    export let language: string;

    article.subscribe(newArticle => {
        currentArticle = newArticle;
    });


    const handleArticleChange = (newArticle: number) => {
        currentArticle = newArticle;
        article.update(() => newArticle);
    };

</script>

<main
    class="main"
>
    <article
        id="article"
        class="content"
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
    <sidebar
        class="articles-list"
    >
        <ul>
            <li on:click={() => handleArticleChange(1)} style={currentArticle === 1 ? 'text-decoration: underline;' : ''} >
                {language === 'es' ? 'Por qué perspectiva' : 'Why perspective'}
            </li>
            <li on:click={() => handleArticleChange(2)} style={currentArticle === 2 ? 'text-decoration: underline;' : ''}>
                {language === 'es' ? 'Más en un toque' : 'More coming soon'}
            </li>
        </ul>
    </sidebar>
</main>

<style>
    main.main {
        display: flex;
        flex-direction: column-reverse;
        justify-content: flex-end;
    }

    article.content {
        width: 90%;
    }

    sidebar.articles-list ul {
        list-style-type: none;
        padding: 0;
    }

    sidebar.articles-list ul li {
        margin: .5rem 0;
    }

    sidebar.articles-list ul li:hover {
        margin: .5rem 0;
        cursor: pointer;
        text-decoration: underline;
    }

    @media screen and (min-width: 480px) {
        main.main {
            padding: 5rem 12rem;
            flex-direction: row;
            justify-content: space-between;
        }

        article.content {
            font-size: 1.2rem;
            width: 60%;
        }

        sidebar.articles-list ul li {
            text-decoration: none;
        }
    }
</style>