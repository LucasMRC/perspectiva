<script lang="ts">
    import Article from './articles/article.svelte';
	import { article, locale } from '@utils/stores';

    const handleArticleChange = (newArticle: number) => {
        article.set(newArticle);
    };

</script>

<main
    class="main"
>
    <article
        id="article"
        class="content"
    >
        <Article />
    </article>
    <sidebar
        class="articles-list"
    >
        <ul>
            <li>
                <button on:click={() => handleArticleChange(1)} style={$article === 1 ? 'text-decoration: underline;' : ''} >
                    {$locale === 'es' ? 'Por qué perspectiva' : 'Why perspective'}
                </button>
            </li>
            <li>
                <button on:click={() => handleArticleChange(2)} style={$article === 2 ? 'text-decoration: underline;' : ''}>
                    {$locale === 'es' ? 'Más en un toque' : 'More coming soon'}
                </button>
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

    sidebar.articles-list > ul {
        list-style-type: none;
        padding: 0;
    }

    sidebar.articles-list > ul > li {
        margin: .5rem 0;
    }

    sidebar.articles-list > ul > li > button {
        background: transparent;
        padding: 0;
        border: none;
    }

    sidebar.articles-list > ul > li > button:hover {
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

        sidebar.articles-list > ul > li > button {
            text-decoration: none;
        }
    }
</style>