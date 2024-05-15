<script>
    // Exporting properties for dynamic usage
    export let href; // Link URL
    export let text; // Link text
    export let type; // Type of button (primary, secondary, secondary-black)
</script>

<!-- Link element with dynamic class and href -->
<a class="{type}" href="{href}">{text}</a>

<!-- Styles -->
<style>
    /* Default styling for links */
    a {
        padding: 16px 36px;
        font-weight: 500;
        color: white;
        border-radius: 50px;
        font-size: var(--fs-400);
        transition: 200ms all ease-out;
    }

    /* Primary button styling */
    .primary {
        background: var(--gradient);
    }

    /* Secondary button styling */
    .secondary {
        border: 2pt solid white;
    }

    /* Secondary-black button styling */
    .secondary-black {
        color: var(--dark);
        border: 2pt solid var(--dark);
    }

    /* Hover effect for links */
    a:hover {
        background: var(--dark);
        color: white;
        transform: scale(0.97); /* Fixed the property name from 'scale' to 'transform' */
    }

    /* Active state effect for links */
    a:active {
        transform: scale(0.95); /* Fixed the property name from 'scale' to 'transform' */
    }

    /* Media query for smaller screens */
    @media screen and (max-width: 768px) {
        a {
            padding: 12px 28px; /* Adjusted padding for smaller screens */
        }
    }
</style>
