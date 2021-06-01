<script>
  import { createEventDispatcher } from 'svelte';
  import { slide, fade } from 'svelte/transition';

  const dispatch = createEventDispatcher();

  function closeMenu() {
    dispatch('closemenu');
  }
</script>

<div class="container" transition:slide>
  <ul>
    <li>
      <a href="#aboutme" transition:fade on:click={closeMenu}>About</a>
    </li>
    <li>
      <a href="#projectgrid" transition:fade on:click={closeMenu}>Blogs</a>
    </li>
    <li>
      <a href="#projectgrid" transition:fade on:click={closeMenu}>Projects</a>
    </li>
    <li>
      <a href="#prevexp" transition:fade on:click={closeMenu}>Experience</a>
    </li>
    <li>
      <a href="#contact" transition:fade on:click={closeMenu}>Contact</a>
    </li>
  </ul>
</div>

<style>
  .container {
    margin-top: 3rem;
    padding-top: 0;
    height: 360px;
    width: 100%;
    background-color: rgb(77, 77, 77);
    position: fixed;
    z-index: 1;
    border-bottom-left-radius: 5%;
    border-bottom-right-radius: 5%;
  }
  ul {
    padding: 0;
    margin: auto;
    margin-top: 1rem;
    width: 100%;
  }
  li {
    list-style: none;
    text-align: center;
  }
  a {
    text-decoration: none;
    color: white;
    font-size: 2.5rem;
  }
</style>
