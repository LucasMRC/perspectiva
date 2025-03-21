<script lang="ts">
    import { locale } from '../../../utils/stores';

    export let showMenu: boolean;
</script>

<div
    id="menu-container"
    style="
        opacity: {showMenu ? '1' : '0'};
        pointer-events: {showMenu ? 'all' : 'none'};"
>
    <ul
        class="menu-list"
    >
        <li
            class="menu-item"
        >
            <a
                href="#article"
            >
                {$locale === 'es' ? 'Artículos' : 'Articles'}
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
</style>
