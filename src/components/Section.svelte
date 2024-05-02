<script>
    export let title
    export let inhalt
    export let type
    export let buttonLink
    export let buttonText
    export let buttonType

    import Button from "./Button.svelte";
</script>

<section class="{type}">
    <article>
        <h1>{title}</h1>
        <p>{inhalt}</p>
        <Button link="{buttonLink}" text={buttonText} type={buttonType}/>
    </article>
</section>  


<style>
    section{
        margin-top: 100px;
        width: 100%;
        display: flex;
    }


    article{
        width: 1120px;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        gap: 3rem;
        padding: 80px 0px;
    }

    .primary{
        background-color: var(--primary);
    }

    .primary article h1{
        color: white;
        font-size: 36px;
    }

    .primary article p{
        font-size: 16px;
        text-align: center;
        color: #EBEBEB;
    }
</style>