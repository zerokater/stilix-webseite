<script>
    export let title
    export let copy

    import { slide } from "svelte/transition";

    let isOpen = false;
    let rotation = 0;

    function toggle(){
        isOpen = !isOpen;
        rotation = isOpen ? 45 : 0;
    }
</script>

<div class="service">
    <div class="title">
        <h4>{title}</h4>
        <img class="svg-icon" on:click={toggle} src="images/close-plus.svg" alt="" style="transform: rotate({rotation}deg);">
    </div>
    {#if isOpen}
        <div class="copy" transition:slide>
            <p>{copy}</p>
        </div>
    {/if}
</div>


<style>

    .title{
        display: flex;
        justify-content: space-between;
    }

    .service{
        padding: 1rem 0rem;
        border-top: 2pt solid var(--white);
        display: flex;
        flex-direction: column;
    }

    h4{
        letter-spacing: 1px;
        color: var(--white);
        font-size: var(--fs-m);
    }

    p{
        width: 90%;
        color: var(--white);
    }

    /* Transition effect for smooth rotation */
    .svg-icon {
        transition: transform 0.3s ease;
    }

    img{
        cursor: pointer;
    }
</style>
