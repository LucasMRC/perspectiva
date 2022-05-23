
<script lang="ts">
    import MenuIcon from "./MenuIcon.svelte";
    import MenuList from "./MenuList.svelte";

    let showMenu = false;

    const handleClickOnMenu = () => {
        showMenu = !showMenu;
    };

</script>

<MenuIcon
    showMenu={showMenu}
    onClick={handleClickOnMenu}
/>
<MenuList
    showMenu={showMenu}
    handleClickOnMenu={handleClickOnMenu}
/>

<style>

</style>