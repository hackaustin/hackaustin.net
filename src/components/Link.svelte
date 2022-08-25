<script>
  export let target;
</script>

<a href={target}><slot></slot></a>

<style>
  a {
    color: white;
    text-decoration: none;
    font-weight: bold;
  }

  a:not(.button > a) {
      box-shadow: inset 0 0 0 0 var(--primary-green);
      margin: 0 -.25rem;
      padding: 0 .25rem;
      transition: color .3s ease-in-out, box-shadow .3s ease-in-out;
  }
  a:not(.button > a):hover {
      box-shadow: inset 100px 0 0 0 var(--primary-green);
      color: black;
  }
</style>
