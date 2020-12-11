<script>
</script>

<style>
  h2 {
    text-align: center;
    padding-bottom: 1rem;
  }
  .container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    width: 90%;
    justify-content: space-around;
    margin: auto;
    gap: 10px;
  }

  .skill {
    /* background-color: lightgrey; */
    width: 175px;
    height: 175px;
    text-align: center;
    background-position: center;
    background-size: contain;
    background-repeat: no-repeat;
  }

  .svelte {
    background-image: url("../assets/skill-logos/Svelte_Logo.svg.png");
  }

  .react {
    background-image: url("../assets/skill-logos/react2.png");
  }

  .deno {
    background-image: url("../assets/skill-logos/Deno.svg.png");
  }

  .node {
    background-image: url("../assets/skill-logos/nodejs.svg");
  }

  .svelte {
    background-image: url("../assets/skill-logos/Svelte_Logo.svg.png");
  }

  .svelte {
    background-image: url("../assets/skill-logos/Svelte_Logo.svg.png");
  }
</style>

<h2>Web Dev Technologies</h2>

<div class="container">
  <div class="skill svelte image" />
  <div class="skill deno" />
  <div class="skill node" />
  <div class="skill react" />
</div>
