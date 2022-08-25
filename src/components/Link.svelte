<script>
  export let target;
</script>

<a href={target}><slot></slot></a>

<style>
  a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    padding-left: 0.5rem;
    padding-right: 0.5rem;
  }

  a:not(.button > a) {
      box-shadow: inset 0 0 0 0 var(--primary-green);
      margin: 0 -.25rem;
      padding: 0 .3rem;
      transition: color .3s ease-in-out, box-shadow .3s ease-in-out;
  }
  a:not(.button > a):hover {
      box-shadow: inset 300px 0 0 0 var(--primary-green);
      color: black;
  }
</style>
