<script>
    import Section from "./Section.svelte";
    import Service from "./Service.svelte";

</script>

<Section>
    <h2>Unsere Services</h2>
    <div class="services">
        <Service title="Grafikdesign" copy="Wir bringen deine Marke zum Leben - von Konzept bis Umsetzung. Ideen werden durch Farben, Formen, Typografie und Bilder zu ansprechenden Designs." />
        <Service title="Webdesign" copy="Wir verwandeln deine Vision in eine Online-Präsenz, die nicht nur ästhetisch ansprechend ist, sondern mit deinem Look & Feel und einer intuitiven Nutzerführung punktet." />
        <Service title="Branding" copy="Wir verleihen deiner Marke mit einem Brand Design ein einheitliches Erscheinungsbild und eine ganzheitliche visuelle Präsenz. Grafikdesign und Webdesign im Komplettpaket."/>
    </div>
</Section>


<style>

    .services{
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }


    h2{
        font-size: var(--fs-l);
        color: var(--white);
    }


</style>