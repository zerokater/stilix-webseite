<section>
    <article>
        <slot></slot>
    </article>
</section>


<style>
    section{
        width: 100%;
    }

    article{
        padding: 2rem 0rem;
        width: 1400px;
        background-color: brown;
        margin: 0 auto;
        height: 40vh;
    }

    @media screen and (max-width: 1460px) {
    article {
        padding: 2rem;
        width: 100%;
    }
    }
</style>