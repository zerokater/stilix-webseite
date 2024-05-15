<script>
    import { slide } from "svelte/transition";

    export let title
    export let copy

    let isMenuOpen = false;

    const toggleMenu = () => {
    isMenuOpen = !isMenuOpen;
    };
</script>

<div class="container">
    <div class="title">
        <h3>{title}</h3>
        <a class="{isMenuOpen ? "close" : "open"}" href="{void(0)}" on:click={toggleMenu}><img src="images/close-plus.svg" alt=""></a>
    </div>
    <div class="copy">
        {#if isMenuOpen}
            <p transition:slide>{copy}</p>
        {/if}
    </div>
</div>

<style>
    .container{
        padding: 1rem 0rem;
        border-top: 2pt solid var(--white);
        width: 1000px;
    }

    .title{
        display: flex;
        justify-content: space-between;
    }

    .container:last-child{
        border-bottom: 2pt solid var(--white);
    }


    h3{
        color: var(--white);
        font-size: var(--fs-m);
        font-weight: 600;
        letter-spacing: 1px;
    }

    p{
        width: 90%;
        font-size: var(--fs-400);
        color: var(--white);
    }

    .close{
        cursor: pointer;
        transition: all 200ms;
    }

    .open{
        cursor: pointer;
        transform: rotate(-45deg);
        transition: all 200ms;
    }


    

    @media screen and (max-width: 1460px) {
    .container {
        padding: 1rem 0rem;
        width: 100%;
    }


    }
    
</style>