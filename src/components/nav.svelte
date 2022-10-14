<script>
    import Link from "/src/components/Link.svelte"
</script>

<nav>
    <h2 class="mono primary-green">HACK<span class="space"></span>AUSTIN!</h2>
    <div class="button-box">
        <Link target="https://bank.hackclub.com/donations/start/hackaustin">Donate</Link>
        <span class="button"><a onlick="window.fathom.trackGoal('BJ9BT1ZU', 0);" href="https://register.hackaustin.net">Register!</a></span>
    </div>
    
    
</nav>

<style>
    nav {
        position: fixed;
        display: flex;
        background-color: black;
        height: max-content;
        width: 100vw;
        top: 0;
        padding:0.5rem;
        padding-right: 2rem;
        box-sizing: border-box; 
        line-height: 2rem;
        color: white;
        align-items: center;
        z-index: 1;
    }
    
    a {
        text-decoration: none;
        font-weight: 700;
    }

    h2 {
        margin: 0;
        font-size: 5vmin;
        line-height:5vmin; 
    }
    
    .space {
        display: inline-block;
        width: 0.5rem;
        height: 1rem;
    }

    .button {
        display: inline-flex;
        justify-content: center;
        background: var(--primary-green);
        color: black;
        border-radius: 2.5px;
        padding: 0.5rem;
        transition: ease 0.25s;
        cursor: pointer;
        user-select: none;
    }

    .button > a {
        color: black;
        margin:0;
        line-height: 1rem;
    }

    .button:hover {
        transform: translateX(-0.25em);
    }

    .button:active {
        transform: scale(0.98);
    }

    .button-box {
        display:flex;
        justify-content:end;
        flex-grow: 4;
        gap:1.5rem;
        font-size:1.25rem;
    }
</style>
