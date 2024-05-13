<script>
    import Button from "../components/Button.svelte";
    import Section from "../components/Section.svelte";
    import { blur  } from "svelte/transition";
</script>

<main transition:blur>
    <article>
        <h1>Kreatives design <br> für <span>starke Marken</span></h1>
        <p>Stilix ist eine Kreativagentur, die Unternehmen hilft, sich als Branchenführer zu profilieren.</p>
        <Button href="/kontakt" text="Los geht's"/>
    </article>
</main>

<!--.
<Section>
    <h1>alo</h1>
    <a href="/">che fai</a>
</Section>
-->

<style>
    main{
        width: 100%;
        background-color: var(--dark);
        display: flex;
        justify-content: center;
        align-items: center;
    }

    article{
        padding: 2rem 0rem;
        width: 1400px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 500px;
        gap: 1.5rem;
    }

    
    h1{
        font-size: var(--h1);
        text-align: center;
        line-height: 130%;
        color: white;
    }

    span{
        background: var(--gradient);;
        background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    p{
        width: 500px;
        color: var(--gray);
        text-align: center;
    }

















    @media screen and (max-width: 1460px) {
        article {
            padding: 2rem;
            width: 100%;
        }
    }

    @media screen and (max-width: 768px) {

        article{
            align-items: start;
        }
        h1 {
            font-size: 40px;
            text-align: start;
        }

        p{
            width: auto;
            text-align: start;
        }
    }
</style>