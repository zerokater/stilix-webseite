<header>
    <nav>
        <img src="images/stilix-logo-sw.svg" alt="">
        <nav-links>
            <a href="/">Über uns</a>
            <a class="cta" href="/">Kontakt</a>
        </nav-links>
    </nav>
</header>

<style>
    header{
        width: 1120px;
        padding: 3rem 0rem;
        margin: 0 auto;

    }

    nav{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    nav-links{
        display: flex;
        gap: 2rem;
        justify-content: center;
        align-items: center;
        font-weight: 500;
    }

    nav-links a{
        color: var(--secondary);
        transition: all 0.15s;
    }

    nav-links    a:hover{
        color: var(--primary);
    }

    .cta{
        padding: 1rem 2rem;
        border-radius: 0.3rem;
        color: #ffffff;
        background-color: var(--secondary);
        font-weight:600;
        transition: all 0.15s;
    }

    .cta:hover{
        background-color: var(--primary);
        color: #ffffff;
    }

    img{
        width: 120px;
    }
    

</style>