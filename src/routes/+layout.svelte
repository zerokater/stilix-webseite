<script>
    import Nav from "/src/components/Nav.svelte";

</script>


<Nav/>


<slot/>


<style>
   @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');


   :global(*){
    font-family: "Poppins", sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    text-decoration: none;
    color: var(--dark);
   }

   :global(:root){
    --primary: #ef233c;
    --dark: #050505;
    --gray: #8E9095;
    --green:#00ce2d;
    --blue: #2187E7;
    --white: #fff;
    --gradient: linear-gradient(120deg, #9d00ff, #0099f8);
    --gradient-green: linear-gradient(120deg, #08FFF0, #60FF4E);


    --fs-xl: clamp(.875rem, 8vw, 5rem);
    --fs-l: clamp(.875rem, 6vw, 3rem);
    --fs-m: clamp(.875rem, 4vw, 1.5rem);
    --fs-400: clamp(15px, 3vw, 16px);
   }




   :global(html){
        scroll-behavior: smooth;
   }

</style>