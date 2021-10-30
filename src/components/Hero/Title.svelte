<script lang="ts">
    import { onMount } from "svelte";

    const fullTitle = 'Perspectiva';
    // let title = '';
    // let count = 0;
    // const interval = setInterval(() => {
    //     title = fullTitle.slice(0, count++);
    //     if (title === fullTitle) clearInterval(interval);
    // }, 100);
    onMount(() => {
        const titleElement = document.querySelector('h1.title') as HTMLHeadingElement;
        setTimeout(() => titleElement.style.opacity = '.5', 0);
    });
    
</script>

<h1 class="title">
    {fullTitle}
</h1>

<style>

    h1.title {
        margin: 2rem 15rem 0;
        font-size: 8rem;
        font-weight: 100;
        text-transform: uppercase;
        letter-spacing: -0.6rem;
        text-align: center;
        transition: opacity ease 2300ms;
        opacity: 0;
    }

    h1.title::after {
        content: 'by Luki';
        text-transform: none;
        font-size: 1rem;
        color: var(--secondary-color);
        letter-spacing: .2rem;
        position: relative;
        top:1rem;
        right: 6rem;
        text-shadow: 0 .125rem .25rem #000;
        font-weight: var(--regular-font);
    }

</style>