<script lang="ts">
    export let showMenu: boolean;
    export let onClick: () => void;
</script>

<div
    on:click={onClick}
    role="button"
    tabindex="0"
    on:keydown={() => {}}
    aria-label="Menu icon"
    class={showMenu ? 'is-active' : ''}
    id="menu-icon"
>
    <span class="line" />
    <span class="line" />
    <span class="line" />
</div>

<style>
    #menu-icon {
        position: absolute;
        left: 3rem;
        top: 3rem;
        width: 3rem;
        background: transparent;
        border: none;
    }

    #menu-icon,
    #menu-icon .line {
        -webkit-transition: all 0.5s cubic-bezier(0.71,-0.07, 0.74, 1.21);
        -o-transition: all 0.5s cubic-bezier(0.71,-0.07, 0.74, 1.21);
        transition: all 0.5s cubic-bezier(0.71,-0.07, 0.74, 1.21);
    }

    #menu-icon .line {
        width: 25px;
        height: 1px;
        background-color: var(--primary-color);
        opacity: .5;
        display: block;
        margin: 8px auto;
    }

    #menu-icon:hover {
        cursor: pointer;
    }

    #menu-icon.is-active {
        width: 60px;
        height: 90px;
    }

    #menu-icon.is-active .line:nth-child(2) {
        -webkit-transform: translateX(-25px) rotate(90deg);
        -ms-transform: translateX(-25px) rotate(90deg);
        -o-transform: translateX(-25px) rotate(90deg);
        transform: translateX(-25px) rotate(90deg);
        transform-origin: 0 0;
        width: 25px; /* 30px * articles in the list */
    }

    #menu-icon.is-active .line:nth-child(1) {
        margin-bottom: 0;
        width: 65px;
    }

    #menu-icon.is-active .line:nth-child(3) {
        margin-top: 0;
        -webkit-transform: translateX(-25px) rotate(90deg) ;
        -ms-transform: translateX(-25px) rotate(90deg) ;
        -o-transform: translateX(-25px) rotate(90deg) ;
        transform: translateX(-25px) rotate(90deg) ;
        transform-origin: 0 0;
        width: 0px;
    }
</style>