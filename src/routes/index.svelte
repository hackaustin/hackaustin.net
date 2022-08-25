<script>
    import Hero from "../components/hero.svelte"
    import Splash from "../components/splash.svelte";
    import Nav from "../components/nav.svelte";
    import About from "../components/about.svelte"
    import Link from "../components/Link.svelte";
</script>

<svelte:head>
  <!-- HTML Meta Tags -->
  <title>Hack Austin!</title>
  <meta name="description" content="Hack Austin is a nonprofit hackathon for Austin high-schoolers to learn to code and build projects they're proud of. The venue is TBD, and will be held on October 14th from 10AM-8PM. Register today!">

  <!-- Google / Search Engine Tags -->
  <meta itemprop="name" content="Hack Austin!">
  <meta itemprop="description" content="Hack Austin is a nonprofit hackathon for Austin high-schoolers to learn to code and build projects they're proud of. The venue is TBD, and will be held on October 14th from 10AM-8PM. Register today!">
  <meta itemprop="image" content="/meta.png">

  <!-- Facebook Meta Tags -->
  <meta property="og:url" content="https://hackaustin.net">
  <meta property="og:type" content="website">
  <meta property="og:title" content="Hack Austin!">
  <meta property="og:description" content="Hack Austin is a nonprofit hackathon for Austin high-schoolers to learn to code and build projects they're proud of. The venue is TBD, and will be held on October 14th from 10AM-8PM. Register today!">
  <meta property="og:image" content="/meta.png">

  <!-- Twitter Meta Tags -->
  <meta name="twitter:card" content="summary_large_image">
  <meta name="twitter:title" content="Hack Austin!">
  <meta name="twitter:description" content="Hack Austin is a nonprofit hackathon for Austin high-schoolers to learn to code and build projects they're proud of. The venue is TBD, and will be held on October 14th from 10AM-8PM. Register today!">
  <meta name="twitter:image" content="/meta.png">
</svelte:head>

<Nav/>
<Hero/>
<Splash/>

<footer>
    <h2>For questions, concerns, etc. , or just to talk coding, contact <Link target="mailto://team@hackaustin.net">team@hackaustin.net</Link>! </h2>
</footer>

<style>
    footer {
        display: flex;
        background-color: black;
        justify-content: center;
        color: white;
    }
    
    footer > h2 {
        text-align: center;
    }
    
    
</style>
