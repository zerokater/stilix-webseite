<script>
    import { onMount } from 'svelte';
  
    import { slide } from 'svelte/transition';
    import { quintOut } from 'svelte/easing';

    let isSmallScreen = false;
    let isMenuOpen = false;
  
    
    const checkScreenSize = () => {
      isSmallScreen = window.innerWidth <= 768; // Anpassen der Breakpoint-Größe bei Bedarf
    };
  
    onMount(() => {
      checkScreenSize();
      window.addEventListener('resize', checkScreenSize);
      return () => window.removeEventListener('resize', checkScreenSize);
    });
  
    const toggleMenu = () => {
      isMenuOpen = !isMenuOpen;
    };
</script>

<header>

    <nav>
        {#if isMenuOpen & isSmallScreen}
            <img id="logo" src="images/stilix-logo-negativ.svg" alt=""> 
        {:else}
             <img id="logo" src="images/stilix-logo-negativ.svg" alt="">
        {/if}
    
        {#if isSmallScreen}
            <!-- Small screen menu (e.g., hamburger menu) -->
            {#if !isMenuOpen}
                <a id="hamburger" href="/" on:click={toggleMenu}><img src="images/hamburger.svg" alt=""></a>
            {:else}
                <a id="hamburger" href="/" on:click={toggleMenu}><img src="images/hamburger-close.svg" alt=""></a>
            {/if}
    
            {#if isMenuOpen}
                <div class="nav-links-hamburger" transition:slide>
                    <a href="/" on:click={toggleMenu}>Home</a>
                    <a href="/" on:click={toggleMenu}>Über Uns</a>
                    <a href="/" on:click={toggleMenu}>Services</a>
                    <a href="/" on:click={toggleMenu}>Kontakt</a>
                </div>
            {/if}
        {:else}
            <!-- Large screen menu -->
            <div class="nav-links">
                <a href="/">Home</a>
                <a href="/">Über Uns</a>
                <a href="/">Services</a>
                <a href="/">Kontakt</a>
            </div>
        {/if}
    </nav>
</header>
  
<style>


    header{
        background-color: var(--dark);
        width: 100%;
      
    }

    #logo{
        z-index: 2;
        width: 84px;
    }


    #hamburger{
        z-index: 2; 
        display: flex;
        align-items: center;
        justify-content: center-;
    }

    #hamburger img{
        width: 32px;
        cursor: pointer;
    }
    /* Add your CSS styling here */
    nav {
        
        padding: 2rem 0rem;
        width: 1400px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center ;
      /* Add styles for the menu container */
    }
  
    .nav-links{
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 2rem;
    }


    .nav-links a{
        color: var(--gray);
    }

    .nav-links a:hover{
        color: white;
    }
    .nav-links-hamburger{
        padding: 0rem 2rem;
        width: 100%;
        height: 100vh;
        overflow: hidden;
        position: fixed;
        top: 0;
        left: 0;
        display: flex;
        justify-content: center;
        align-items: flex-start;
        flex-direction: column;
        gap: 1.5rem;
        background: var(--dark);
    }

    .nav-links-hamburger a{
        z-index: 5;
        font-size: 48px;
        font-weight: 700;
        color: white;
        transition: all 0.2s ease-out;
    }

    .nav-links-hamburger a:hover{
        background: var(--gradient);
        padding: 0rem 10px;
        background-clip: text;
        -webkit-text-fill-color: transparent;
    }
    



    @media screen and (max-width: 1460px) {
    nav {
        padding: 2rem;
        width: 100%;
    }
    }

    /* On screens that are 992px or less, set the background color to blue */
    @media screen and (max-width: 768px) {
    nav {
        padding: 2rem;
        width: 100%;
    }
    }
</style>
  