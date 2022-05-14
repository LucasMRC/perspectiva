<script lang="ts">
    import { onMount } from "svelte";

    const fullTitle = 'Perspectiva';
    onMount(() => {
        const titleElement = document.querySelector('h1.title') as HTMLHeadingElement;
        setTimeout(() => titleElement.style.opacity = '.5', 0);
    });
</script>

<h1 class="title">
    {fullTitle.toUpperCase()}
</h1>

<style>

    h1.title {
        font-weight: 100;
        text-align: center;
        transition: opacity ease 2300ms;
        opacity: 0;
        position: relative;
    }

    h1.title::after {
        content: 'by Luki';
        font-size: 1rem;
        color: var(--secondary-color);
        letter-spacing: .2rem;
        position: absolute;
        top: 2rem;
        right: 3rem;
        text-shadow: 0 .125rem .25rem #000;
        font-weight: var(--regular-font);
    }

    @media screen and (min-width: 480px) {
        h1.title {
            margin: 2rem 15rem 0;
            font-size: 8rem;
            letter-spacing: -0.6rem;
        }

        h1.title::after {
            position: relative;
            top: 1rem;
            right: 6rem;
        }

    }

</style>