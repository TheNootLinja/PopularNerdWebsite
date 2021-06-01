<script>
  export let open = false;
</script>

<aside class:open>
  <nav>
    <a href="#aboutme">About</a>
    <a href="#skills">Skills</a>
    <a href="#skills">Projects</a>
    <a href="#skills">Contact</a>
  </nav>
</aside>

<style>
  a {
    display: block;
  }
  aside {
    left: -100%;
    transition: left 0.3s ease-in-out;
  }
  .open {
    left: 0;
  }
</style>
