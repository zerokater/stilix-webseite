<script>
    export let background
</script>

<section class="{background}">
    <article>
        <slot></slot>
    </article>
</section>


<style>


    section{
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }


    .white{
        background-color: var(--white);
    }

    .dark{
        background-color: var(--dark);
    }

    .gradient{
        background: var(--gradient);
    }

    article{
        display: flex;
        justify-content: center;
        align-items: stretch;
        padding: 5rem 0rem;
        width: 1400px;
        gap: 2rem;
        overflow: hidden;
    }





    @media screen and (max-width: 1460px) {
    article {
        padding: 2rem;
        width: 100%;
    }


    }



    @media screen and (max-width: 600px) {
    article {
        gap: 1rem;
        flex-wrap: wrap;
    }


    }
</style>