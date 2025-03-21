<script lang="ts">
    import { locale } from '../../../utils/stores';
    import Menu from "./Menu.svelte";

    function handleLocaleChange(e: Event) {
        const newLocale = (e.target as HTMLButtonElement).textContent?.toLowerCase();
        locale.set(newLocale ?? 'en');
    }

</script>

<div class="navbar">
    <Menu />
    <div class="locale-container">
        <button class="locale-button" on:click={handleLocaleChange}>ES</button>
        |
        <button class="locale-button" on:click={handleLocaleChange}>EN</button>
    </div>
</div>

<style>
    div.navbar {
        display: flex;
        position: relative;
        align-items: center;
        justify-content: center;
        height: 8.5rem;
    }

    div.locale-container {
        position: absolute;
        right: 3rem;
        top: 3rem;
        user-select: none;
    }

    div.locale-container > button {
        border: none;
        background: transparent;
        cursor: pointer;
    }

    div.locale-container > button:hover {
        text-decoration: underline;
    }
</style>
