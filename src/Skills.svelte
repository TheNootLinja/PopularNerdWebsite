<script>
</script>

<style>
  h2 {
    text-align: center;
    /* padding-bottom: 1rem; */
    margin-top: 15px;
    margin-bottom: 10px;
  }
  p {
    text-align: center;
    margin-bottom: 2rem;
  }

  .container {
    width: 95%;
    margin: auto;
    margin-top: 1.5rem;
  }

  .grid-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    width: 90%;
    justify-content: space-around;
    margin: auto;
    gap: 5px;
  }

  .skill {
    /* background-color: lightgrey; */
    width: 125px;
    height: 125px;
    text-align: center;
    background-position: center;
    background-size: contain;
    background-repeat: no-repeat;
    margin: auto;
  }

  .svelte {
    background-image: url("../assets/skill-logos/Svelte_Logo.svg.png");
  }

  .react {
    background-image: url("../assets/skill-logos/react2.png");
  }

  .deno {
    background-image: url("../assets/skill-logos/Deno.svg.png");
    background-color: white;
    border-radius: 100%;
    margin: auto;
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

  .card {
    padding: 0.4rem;
    padding-top: 1.2rem;
    margin: auto;
    width: 95%;
  }
</style>

<div class="container">
  <h2>My Skills</h2>
  <p>
    I have spent a lot of my time working with React and Svelte on the front
    end, while on the backend the majority of my experience is using Nodejs. I
    also know Deno as I think it will only grow in popularity and I am always
    looking to get ahead of the raging tide that is new things in web
    development.
  </p>

  <div class="grid-container">
    <div class="skill svelte image" />
    <div class="skill deno" />
    <div class="skill node" />
    <div class="skill react" />
  </div>
</div>
