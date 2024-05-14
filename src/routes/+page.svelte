<script>
    import Button from "../components/Button.svelte";
</script>

<main>
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
        width: 1401px;
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

    @media screen and (max-width: 470px) {

    article{
        align-items: start;
        gap: 1rem;
    }
    h1 {
        font-size: 36px;
        text-align: start;
    }

    p{
        font-size: 16px;
        width: auto;
        text-align: start;
    }
    }
</style>