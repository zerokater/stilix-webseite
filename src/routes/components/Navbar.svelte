<header>
    <nav>
        <img src="images/stilix-logo.svg" alt="">
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

    img{
        width: 120px;
    }
    
    .cta{
        cursor: pointer;
        color: #ffffff;
        background-color: var(--primary);
        padding: 1rem 2rem;
        border-radius: 0.5rem;
        transition: 0.2s;
        font-weight: 600;
    }


    .cta:hover{
        scale: 1.05;
    }
</style>