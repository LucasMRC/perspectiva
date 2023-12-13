<script lang="ts">
    const fullTitle = 'Perspectiva';
</script>

<h1 class="title">
    {fullTitle.toUpperCase()}
</h1>

<style>
    @keyframes fade-in {
        0% { opacity: 0; }
        25% { opacity: 0; }
        100% { opacity: .5; }
    }

    h1.title {
        font-weight: 100;
        text-align: center;
        transition: opacity ease 2300ms;
        position: relative;
        opacity: 1;
        animation-name: fade-in;
        animation-duration: 3s;
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
            font-size: 8rem;
            letter-spacing: -0.6rem;
            opacity: .5;
        }

        h1.title::after {
            position: relative;
            top: 1rem;
            right: 6rem;
        }
    }
</style>