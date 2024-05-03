<header>
    <nav>
        <img src="images/stilix-logo.svg" alt="">
        <nav-links>
            <a href="/">Über uns</a>
            <a href="/">Referenzen</a>
            <a href="/kontakt">Kontakt</a>
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
        color: var(--gray);
        transition: all 0.3s;
    }

    nav-links a:hover{
        color: var(--secondary);
    }



    img{
        width: 85px;
    }
    

</style>