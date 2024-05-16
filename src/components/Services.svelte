<script>
    import Service from "./Service.svelte";
</script>

<section>
    <article>
        <h3>Unsere Services</h3>
        <div class="services">
            <Service title="Grafikdesign"/>
            <Service title="Webdesign"/>
            <Service title="Branding"/>
        </div>
    </article>
</section>

<style>
    section{
        width: 100%;
        display: flex;
        justify-content: center;
        background: var(--gradient);
    }

    article{
        padding: 2rem 0rem;
        width: 1400px;
        display: flex;  
        justify-content: center;
        align-items: flex-start;
        flex-direction: row;
        gap: 2rem;
    }

    .services{
        flex: 1;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: stretch;
    }

    h3{
        flex: 1;
        font-size: var(--fs-l);
        color: white;
    }

    @media screen and (max-width: 1460px) {
        article {
            padding: 2rem;
            width: 100%;
        }
    }

    @media screen and (max-width: 768px) {
        article {
            flex-direction: column;
            align-items: stretch;
        }
    }
</style>