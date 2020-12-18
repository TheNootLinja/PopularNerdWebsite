<script>
  import { createEventDispatcher } from "svelte";

  const dispatch = createEventDispatcher();

  export let hbOpen = false;

  function handleHbClick() {
    dispatch("openmenu");
    hbOpen = !hbOpen;
  }
</script>

<style>
  header nav a + a {
    margin-left: 10px;
  }

  /* =========================================================== */

  a {
    display: none;
  }

  .container {
    display: inline-block;
    cursor: pointer;
    margin-top: 8px;
  }
  .last {
    margin-right: 0.5rem;
  }

  .fake-logo {
    font-size: 120%;
    margin: 0;
    margin-left: 0.5rem;
    padding-right: 6px;
    color: #90a9b7;
  }

  .bar1,
  .bar2,
  .bar3 {
    width: 35px;
    height: 5px;
    background-color: #90a9b7;
    margin: 6px 0;
    transition: 0.4s;
  }

  /* Rotate first bar */
  .change .bar1 {
    -webkit-transform: rotate(-45deg) translate(-9px, 6px);
    transform: rotate(-45deg) translate(-9px, 6px);
  }
  /* ==================================================== */
  .nav-icon {
    margin: 1em;
    width: 40px;
  }

  /* Fade out the second bar */
  .change .bar2 {
    opacity: 0;
  }

  /* Rotate last bar */
  .change .bar3 {
    -webkit-transform: rotate(45deg) translate(-8px, -8px);
    transform: rotate(45deg) translate(-8px, -8px);
  }
  /* =========================================================== */
  .last {
    margin-right: 0.5rem;
  }

  .fake-logo {
    font-size: 120%;
    margin: 0;
    margin-left: 0.5rem;
    padding-right: 6px;
    color: #90a9b7;
  }
  @media only screen and (min-width: 500px) {
    a {
      display: inline-block;
    }
    .container {
      display: none;
    }
  }
</style>

<header>
  <h1 class="fake-logo">NRP</h1>
  <nav>
    <div class="container {hbOpen ? 'change' : ''}" on:click={handleHbClick}>
      <div class="bar1" />
      <div class="bar2" />
      <div class="bar3" />
    </div>
    <a href="#aboutme">About</a>
    <a href="#skills">Skills</a>
    <a href="#projectgrid">Projects</a>
    <a href="#contact" class="last">Contact</a>
    <!-- <div class="nav-icon"> -->
    <div />
    <!-- </div> -->
  </nav>
</header>
