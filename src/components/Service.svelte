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
        background-color: var(--white);
        min-width:300px;
        max-width: 400px;
        box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        align-items: center;
        padding: 3rem;
        border-radius: 20px;
        gap: 0.250rem;
        flex-shrink: 1;
    }

    h3{
        text-align: center;
    }

    p{
        text-align: center;
    }


    @media screen and (max-width: 600px) {
    .card {
        max-width: 100%;
    }


    }

</style>