<script>
    import Button from "./Button.svelte";
    import Section from "../components/Section.svelte";
</script>

<main>
    <article>
        <h1>Kreatives design <br> für <span>starke Marken</span></h1>
        <p>Wir sind eine Kreativagentur, die Unternehmen hilft, sich als <br>Branchenführer zu profilieren.</p>
        <Button href="/" text="Los geht's"/>
    </article>
</main>

<Section>
    <h1>alo</h1>
    <a href="/">che fai</a>
</Section>
<style>
    main{
        width: 100%;
        height: 60vh;
        background-color: var(--dark);
    }

    article{
        display: flex;
        padding-top: 10rem;
        width: 1400px;
        margin: auto;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 20px;
    }

    h1{
        text-align: center;
        font-size: 48px;
        color: white;
    }

    p{
        text-align: center;
        color: var(--gray);
        font-size: 16px;
    }

    h1 span{
        background: var(--gradient-green);;
        background-clip: text;
        -webkit-text-fill-color: transparent;
    }



    @media screen and (max-width: 1460px) {
    article {
        padding: 2rem;
        width: 100%;
    }
    }
</style>