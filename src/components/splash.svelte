<script>
import Grid from "./splash-grid.svelte"
import Flex from "./splash-flex.svelte"
</script>

<main>
    <div class="wrapper">
        <h2>Join us and</h2>
        <h1 class="mono">HACK<span class="space"></span>AUSTIN!</h1>
        <div class="grid-container"><Grid/></div>
        <div class="flex-container"><Flex/></div>
   </div>
</main>

<style>
    main {
        min-height:100vh;
        background-color: var(--primary-green);
        color: black;
        display: flex;
        justify-content: center;
        align-items: center;
        padding-top:6rem;
        padding: 2rem;
    }

    h2 {
        margin-top: 0; 
        margin-bottom: 0;
        font-size: 3rem;
    }

    h1 {
        margin-top: 0;
        margin-bottom: 40px;
        font-size: 15vmin;
        line-height: 15vmin;
    }

    .flex-container {
        display: none;
    }
    
    .space {
        width: 5vmin;
        display: inline-block;
    }

    @media (max-width: 850px) {
        .grid-container {
            display: none
        }

        .flex-container {
            display: block;
        }
    }

</style>
