<script>
    // Importing the Button component from its file
    import Button from "../components/Button.svelte";
    import Services from "../components/Services.svelte";
</script>

<main>
    <article>
        <!-- Section containing introductory copy -->
        <div class="copy">
            <!-- Main headline -->
            <h1>Kreatives design für<br><span>starke Marken</span></h1>
            <!-- Subtitle -->
            <p>Stilix ist eine Kreativagentur, die Unternehmen hilft, sich als Branchenführer zu profilieren.</p>
        </div>
        <!-- Call to action buttons -->
        <div class="cta">
            <!-- Primary call to action button -->
                <Button href="/kontakt" text="Los geht's" type="primary"/>
            <!-- Secondary call to action button -->
            <Button href="/services" text="Mehr erfahren" type="secondary-black"/>
        </div>
    </article>
</main>



<Services/>


<!-- Styles -->
<style>
    main {
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    article {
        padding: 10rem 0rem 5rem 0rem;
        width: 1400px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
        gap: 3rem;
    }

    .copy {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 1rem;
    }

    .cta {
        display: flex;
        gap: 2rem;
    }

    h1 {
        font-size: var(--fs-xl);
        line-height: 120%;
        color: var(--dark);
        text-align: center;
    }

    span {
        background: var(--gradient);
        background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    p {
        width: clamp(150px, 450px, 600px);
        font-size: var(--fs-400);
        color: var(--gray);
        text-align: center;
        font-weight: 500;
    }

    /* Media queries for responsiveness */

    @media screen and (max-width: 1460px) {
        article {
            padding: 7rem 2rem 7rem 2rem;
            width: 100%;
        }
    }

    @media screen and (max-width: 768px) {
        article {
            padding: 5rem 2rem 4rem 2rem;
            width: 100%;
        }
        
        p {
            width: 400px;
        }

        .cta {
            gap: 1rem;
        }
    }

    @media screen and (max-width: 470px) {


        p {
            width: auto;
        }
    }
</style>
