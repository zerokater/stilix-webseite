<script>
    export let href
    export let text
    export let type

</script>

<a class="{type}" href="{href}">{text}</a>

<style>

    a{
        padding: 16px 40px;
        font-weight: 500;
        color: white;
        border-radius: 50px;
        font-size: var(--fs-400);
        transition: 200ms all ease-out;
    }

    .primary{
        background: var(--gradient);
    }


    .secondary{
        border: 2pt solid white;
    }

    .secondary-black{
        color: var(--dark);
        border: 2pt solid var(--dark);
    }

    a:hover{
        background: var(--dark);
        color: white;
        scale: 0.97;
        
    }

    a:active{
        scale: 0.95;
    }




    @media screen and (max-width: 768px) {

        a{
            padding: 12px 28px;
        }

    }

</style>