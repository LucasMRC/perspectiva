
<script lang="ts">

    setTimeout(() => {
        const menu_icon = document.getElementById('menu-icon');
        menu_icon?.classList.remove('is-active');
    }, 0);
    const handleClickOnMenu = () => {
        const menu_icon = document.getElementById('menu-icon');
        menu_icon?.classList.toggle('is-active');
    }

</script>

<div
    on:click={handleClickOnMenu}
    class="hamburger is-active"
    id="menu-icon"
>
    <span class="line" />
    <span class="line" />
    <span class="line" />
</div> 

<style>

    div.hamburger {
        position: absolute;
        left: 3rem;
        top: 3rem;
        width: 3rem;
        background: transparent;
        border: none;
    }

    .hamburger .line {
        width: 25px;
        height: 2px;
        background-color: var(--primary-color);
        opacity: .5;
        display: block;
        margin: 8px auto;
        -webkit-transition: all 0.3s ease-in-out;
        -o-transition: all 0.3s ease-in-out;
        transition: all 0.3s ease-in-out;
    }

    .hamburger:hover {
        cursor: pointer;
    }

    #menu-icon.is-active {
        -webkit-transition: all 0.3s ease-in-out;
        -o-transition: all 0.3s ease-in-out;
        transition: all 0.3s ease-in-out;
        -webkit-transition-delay: 0.6s;
        -o-transition-delay: 0.6s;
        transition-delay: 0.6s;
        -webkit-transform: rotate(45deg);
        -ms-transform: rotate(45deg);
        -o-transform: rotate(45deg);
        transform: rotate(45deg);
    }

    #menu-icon.is-active .line:nth-child(2) {
        width: 0px;
    }

    #menu-icon.is-active .line:nth-child(1),
    #menu-icon.is-active .line:nth-child(3) {
        -webkit-transition-delay: 0.3s;
        -o-transition-delay: 0.3s;
        transition-delay: 0.3s;
    }

    #menu-icon.is-active .line:nth-child(1) {
        -webkit-transform: translateY(6px);
        -ms-transform: translateY(6px);
        -o-transform: translateY(6px);
        transform: translateY(6px);
    }

    #menu-icon.is-active .line:nth-child(3) {
        -webkit-transform: translateY(-15px) rotate(90deg);
        -ms-transform: translateY(-15px) rotate(90deg);
        -o-transform: translateY(-15px) rotate(90deg);
        transform: translateY(-15px) rotate(90deg);
    }

</style>