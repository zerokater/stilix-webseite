
<script>
    export let link
    export let text
    export let type 
</script>

<a href="{link}" class="{type}">{text}</a> 

<style>

    a{
        padding: 15px 25px;
        border-radius: 10px;
        transition: all 0.2s;
        font-weight: 500;
    }

    .primary{
        background-color: var(--primary);
        box-shadow: 0 0 40px 5px  rgba(239, 35, 60, 0.5);
        color: white;
    }

    .secondary{
        background-color: white;
        box-shadow: 0 0 40px 5px rgba(255, 255, 255, 0.5);
        color: var(--primary);
    }

    a:hover{
        scale: 0.99;
        box-shadow: none;
    }

    a:active{
        scale: 0.97;
    }
</style>