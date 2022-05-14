
<script lang="ts">
    import MenuIcon from "./MenuIcon.svelte";
    import MenuList from "./MenuList.svelte";

    setTimeout(() => {
        const menu_icon = document.getElementById('menu-icon');
        menu_icon?.classList.remove('is-active');
    }, 0);
    const handleClickOnMenu = () => {
        const menu_icon = document.getElementById('menu-icon');
        menu_icon?.classList.toggle('is-active');
    }

</script>

<MenuIcon />
<MenuList />

<style>

</style>