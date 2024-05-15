<script>
    import Button from "../components/Button.svelte";
</script>

<main>
    <article>
        <div class="copy">
            <h1>Kreatives design für<br><span>starke Marken</span></h1>
            <p>Stilix ist eine Kreativagentur, die Unternehmen hilft, sich als Branchenführer zu profilieren.</p>
        </div>
        <div class="cta">
            <Button href="/kontakt" text="Los geht's" type="primary"/>
            <Button href="/services" text="Mehr erfahren" type="secondary-black"/>
        </div>
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
        display: flex;
        justify-content: center;
        align-items: center;

    }

    article{
        padding: 5rem 0rem;
        width: 1400px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        gap: 3rem;

    }

    .copy{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 1rem;
    }


    .cta{
        display: flex;
        gap: 2rem;
    }


    h1{
        font-size: var(--fs-xl);
        line-height: 120%;
        color: var(--dark);
        text-align: center;
    }

    span{
        background: var(--gradient);;
        background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    p{
        width: clamp(150px, 450px, 600px); 
        font-size: var(--fs-400);
        color: var(--dark);
        text-align: center;
    }















    

    @media screen and (max-width: 1460px) {
        article {
            padding: 10rem 2rem;
            width: 100%;
        }
    }

    @media screen and (max-width: 768px) {
        p{
            width: 400px;
        }

        .cta{
            gap: 1rem;
        }
        

    }


    @media screen and (max-width: 470px) {


        article{
            align-items: flex-start;
            gap: 2rem;
        }

        h1{
            text-align: start;
        }

        p{ 
            text-align: start;
            width: auto;
        }
    }
</style>