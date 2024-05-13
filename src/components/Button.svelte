<script>
    export let href
    export let text


</script>

<a href="{href}">{text}</a>

<style>
    a{
        padding: 15px 35px;
        background: var(--gradient);
        font-weight: 500;
        color: white;
        border-radius: 10px;
        font-size: 16px;
        transition: 200ms all ease-out;
    }

    a:hover{
        background: white;
        color: black;
        scale: 0.97;
    }

    a:active{
        scale: 0.95;
    }
</style>