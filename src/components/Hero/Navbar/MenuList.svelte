
<script lang="ts">

    import { article } from '../../../utils/stores';

    const handleArticleChange = (newArticle: number) => {
        currentArticle = newArticle;
        article.update(() => newArticle);
        handleClickOnMenu();
    };

    export let handleClickOnMenu: () => void;
    export let showMenu: boolean;

    let currentArticle = 1;

</script>

<div
    id="menu-container"
    style="opacity: {showMenu ? '1' : '0'};
            pointer-events: {showMenu ? 'all' : 'none'};"
>
    <ul
        class="menu-list"
    >
        <li
            class="menu-item"
            on:click={() => handleArticleChange(1)}
        >
            <a
                href="#article"
                style={currentArticle === 1 ? 'text-decoration: underline;' : ''}
            >
                Por qué perspectiva
            </a>
        </li>
        <li
            class="menu-item"
            on:click={() => handleArticleChange(2)}
        >
            <a
                href="#article"
                style={currentArticle === 2 ? 'text-decoration: underline;' : ''}
            >
                Más en un toque
            </a>
        </li>
    </ul>
</div> 

<style>
    div#menu-container {
        position: absolute;
        top: 4rem;
        left: 2rem;
        transition: opacity .3s ease-in-out;
        -webkit-transition: opacity 0.3s ease-in-out;
        -o-transition: opacity 0.3s ease-in-out;
    }

    ul.menu-list {
        list-style-type: none;
        padding: 0 1rem .5rem;
        margin: 0;
    }

    li.menu-item {
        line-height: 2rem;
    }

    li.menu-item a {
        text-decoration: none;
        color: var(--primary-light);
    }
</style>