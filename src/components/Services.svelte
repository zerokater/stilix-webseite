<script>
    import Service from "./Service.svelte";
</script>

<section>
    <article>
        <h3>Unsere Services</h3>
        <div class="services">
            <Service title="Grafikdesign" copy="Von Idee bis Design: Deine Marke lebt durch unsere Kreationen. Farben, Formen, Typografie und Bilder machen sie einzigartig."/>
            <Service title="Webdesign" copy="Deine Vision wird zu einer beeindruckenden Online-Präsenz: Ästhetik, Look & Feel und intuitive Nutzerführung vereint."/>
            <Service title="Branding" copy="Einheitliches Brand Design für deine Marke: Grafik- und Webdesign im Komplettpaket."/>
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
        padding: 5rem 0rem;
        width: 1400px;
        display: flex;  
        justify-content: center;
        align-items: flex-start;
        flex-direction: row;
        gap: 2rem;
    }

    .services{
        flex: 2;
        align-self: stretch;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: stretch;
    }

    .services:last-child{
        border-bottom: 2pt solid var(--white);
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
            align-items: center;
            justify-content: center;
        }
    }
</style>