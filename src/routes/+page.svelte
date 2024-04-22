<script>
    import Services from "./components/Services.svelte";
</script>

<main>
    <article>
        <h1>Von der <span>Kreation neuer Marken</span> bis hin zum kleinsten Detail im <span>Design</span></h1>
        <h2>Stilix ist eine Kreativagentur, die Unternehmen hilft, sich von der Masse abzuheben</h2>
    </article>
</main>

<Services/>

<style>
    
    main{
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

    span{

        text-decoration: underline var(--primary);
    }

    h1{
        text-align: center;
        font-size: 48px;
    }
    
    h2{
        font-weight: 500;
    }


</style>