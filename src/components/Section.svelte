<section>
    <article>
        <slot></slot>
    </article>
</section>


<style>
    section{
        width: 100%;
        background: var(--gradient);
    }

    article{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        padding: 5rem 0rem;
        width: 1400px;
        margin: 0 auto;
        gap: 2rem;
        height: 600px;
    }


    @media screen and (max-width: 1460px) {
    article {
        padding: 2rem;
        width: 100%;
    }


    }
</style>