<script>
    // Importing the Button component from its file
    import Service from "../components/Service.svelte";
</script>

<main>
    <article>
        <Service background="/services/livoreka_mockup.jpg" title="Livoreka Bau" service="Grafikdesign"/>
        <Service background="/services/taffa.jpg" title="Taffa Costruzioni" service="Grafikdesign, Branding"/>
        <Service background="/services/restaurant-tsv.png" title="Restaurant TSV" service="Webdesign, Branding"/>
    </article>

</main>




<!-- Styles -->
<style>


    main {
        width: 100%;
        display: flex;
        justify-content: center;
    }

    article{
        width: 1400px;
        display: grid;
        grid-template-columns: repeat(3, minmax(100px, 1fr)); /* Drei Spalten, die sich flexibel anpassen */
        gap: 24px; /* Abstand zwischen den Elementen */
    }

    /* Media queries for responsiveness */

    @media screen and (max-width: 1460px) {
        article{
            width: 95%;
        }
    }

    @media screen and (max-width: 1200px) {
        article{
            grid-template-columns: repeat(2, minmax(100px, 1fr)); /* Drei Spalten, die sich flexibel anpassen */
        }
    }

    @media screen and (max-width: 770px) {
        article{
            grid-template-columns: repeat(1, minmax(100px, 1fr)); /* Drei Spalten, die sich flexibel anpassen */
        }
    }

    @media screen and (max-width: 470px) {


    }
</style>
