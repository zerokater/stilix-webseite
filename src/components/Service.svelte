<script>
    export let src
    export let title
    export let copy
</script>






<div class="card">
    <img src="{src}" alt="">
    <h3>{title}</h3>
    <p>{copy}</p>
</div>

<style>
    .card{
        min-width:300px;
        max-width: 500px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        padding: 3rem;
        border-radius: 20px;
        gap: 1rem;
        flex-shrink: 1;
    }

    h3{

        font-size: var(--fs-m);
        text-align: center;
        color: var(--dark);

    }

    p{
        text-align: center;
        color: var(--gray);

    }


    @media screen and (max-width: 600px) {
    .card {
        max-width: 100%;
    }


    }

</style>