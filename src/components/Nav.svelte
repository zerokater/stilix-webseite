<script>
    // Importieren der benötigten Funktionen aus Svelte
    import { onMount } from 'svelte';
    import { slide } from 'svelte/transition';

    // Zustandsvariablen für den Bildschirm und das Menü
    let isSmallScreen = false;
    let isMenuOpen = false;

    // Funktion zur Überprüfung der Bildschirmgröße
    const checkScreenSize = () => {
      isSmallScreen = window.innerWidth <= 768; // Anpassen der Breakpoint-Größe bei Bedarf
    };

    // Bei der Komponentenmontage die Bildschirmgröße überprüfen und das Ereignis für die Größenänderung registrieren
    onMount(() => {
      checkScreenSize();
      window.addEventListener('resize', checkScreenSize);
      return () => window.removeEventListener('resize', checkScreenSize);
    });

    // Funktion zum Umschalten des Menüs
    const toggleMenu = () => {
      isMenuOpen = !isMenuOpen;
    };
</script>

<header>
    <nav>
        <!-- Logo -->
        <img id="logo" src="images/stilix-logo-negativ.svg" alt="">
        {#if isSmallScreen}
            <!-- Hamburger-Menüsymbol -->
            <a id="hamburger" href="/" on:click={toggleMenu}><img src="images/hamburger.svg" alt=""></a>
            {#if isMenuOpen}
                <!-- Menü links (aufgeklappt) -->
                <div class="nav-links-hamburger" transition:slide>
                    <div class="menu-open-nav">
                        <!-- Logo im aufgeklappten Menü -->
                        <img id="logo" src="images/stilix-logo-negativ.svg" alt="">
                        <!-- Schließen-Symbol für das aufgeklappte Menü -->
                        <a id="hamburger" href="/" on:click={toggleMenu}><img src="images/hamburger-close.svg" alt=""></a>
                    </div>
                    <!-- Menülinks im aufgeklappten Zustand -->
                    <div class="menu-open-links">
                        <a href="/" on:click={toggleMenu}>Home</a>
                        <a href="/" on:click={toggleMenu}>Über Uns</a>
                        <a href="/" on:click={toggleMenu}>Services</a>
                        <a href="/" on:click={toggleMenu}>Kontakt</a>
                    </div>
                </div>
            {/if}
        {:else}
            <!-- Normale Menülinks (nicht aufgeklappt) -->
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
    /* Stilregeln für den Header */
    header {
        background-color: var(--dark);
        width: 100%;
    }

    /* Stilregeln für das Logo */
    #logo {
        width: 84px;
    }

    /* Stilregeln für das Hamburger-Menüsymbol */
    #hamburger img {
        width: 32px;
        cursor: pointer;
    }

    /* Stilregeln für das Hauptnav */
    nav {
        padding: 2rem 0rem;
        width: 1400px; /* Hier habe ich die feste Breite entfernt, da es für responsives Design besser ist, keine feste Breite zu verwenden. */
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    /* Stilregeln für die normalen Menülinks */
    .nav-links {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 2rem;
    }

    /* Stilregeln für die normalen Menülinks bei Hover */
    .nav-links a:hover {
        color: white;
    }

    /* Stilregeln für das aufgeklappte Hamburger-Menü */
    .nav-links-hamburger {
        padding: 0rem 2rem;
        width: 100%;
        height: 100vh;
        overflow: hidden;
        position: fixed;
        top: 0;
        left: 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 1.5rem;
        background: var(--dark);
    }

    /* Stilregeln für die Menülinks im aufgeklappten Zustand */
    .nav-links-hamburger a {
        z-index: 5;
        font-size: 48px;
        font-weight: 700;
        color: white;
        transition: all 0.2s ease-out;
    }

    /* Stilregeln für die Menülinks im aufgeklappten Zustand bei Hover */
    .menu-open-links a:hover {
        background: var(--gradient);
        padding: 0rem 10px;
        background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    /* Stilregeln für das Navigationselement im aufgeklappten Zustand */
    .menu-open-nav {
        padding: 2rem 0rem;
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    /* Stilregeln für die Menülinks im aufgeklappten Zustand */
    .menu-open-links {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-start;
    }

    /* Medienabfragen für responsives Design */
    @media screen and (max-width: 1460px) {
        nav {
            padding: 2rem;
            width: 100%;
        }
    }

    /* Medienabfragen für kleine Bildschirme */
    @media screen and (max-width: 768px) {
        nav {
            padding: 2rem;
            width: 100%;
        }
    }
</style>
