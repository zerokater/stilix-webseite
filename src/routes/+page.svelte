<script>
    import Services from "./components/Services.svelte";
    import Button from "./components/Button.svelte";
    import Section from "./components/Section.svelte";
</script>




<main>
    <article>
        <h1>Von der Kreation neuer Marken bis hin zum<br>kleinsten Detail im Design </h1>
        <h2>Stilix ist eine Kreativagentur, die Unternehmen hilft, sich von der Masse abzuheben</h2>
        <Button link="/" text="Werde Sichtbar" type="primary"/>
    </article>
</main>
 
<Services/>
<Section title="Unsere Mission" inhalt="Du möchtest dich zeigen und wahrgenommen werden? Zusammen werden wir deine Werte undZiele visuell darstellen – mit deinem individuellen Branding. 
Branding ist das, was man sehen, fühlen und hören kann, dein Ich in Schrift und Form und dein persönliches Erscheinungsbild. Wir unterstützen dich dabei, dich klar zu positionieren." type="primary" buttonLink="/" buttonText="Kontaktiere Uns" buttonType="secondary"/>




<style>
    
    main{
        margin-top: 50px;
        width: 100%;
        display: flex;
    }


    article{
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        width: 1120px;
        margin: 0 auto;
        height: 400px;
        gap: 2rem;

    }

    h1{
        text-align: center;
        font-size: 36px;
    }
    
    h2{
        color: var(--gray);
        font-size: 20px;
        font-weight: 400;
    }



</style>