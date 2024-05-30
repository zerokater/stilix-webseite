<script>
    export let background
    export let title
    export let service
</script>


<div class="service" style="background-image: linear-gradient(to top, rgba(0,0,0,0.9), rgba(255,255,255,0)), url({background});">
    <div class="title">
        <h4>{title}</h4>
    </div>
    <div class="category">
        <p>{service}</p>
    </div>
</div>


<style>





    .service{
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        height: 450px;
        transition: all 200ms ease-in-out;
        border-radius: 16px;
        cursor: pointer;

        display: flex;
        flex-direction: column;
        padding: 0rem 2rem 2rem 2rem;
        
        justify-content: flex-end;
        align-items: flex-start;

        border: 1pt solid gainsboro;
    }


    h4{
        font-size: 32px;
        color: var(--white);
    }

    p{
        background: var(--gradient-green);
        background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    .service:hover{
        transform: scale(0.975);

    }


    @media screen and (max-width: 770px) {
        .service{
            height: 350px;
        }
    }
</style>