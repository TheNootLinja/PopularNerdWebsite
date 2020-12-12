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
  }
  .container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    width: 90%;
    justify-content: space-around;
    margin: auto;
    gap: 5px;
  }

  .skill {
    /* background-color: lightgrey; */
    width: 130px;
    height: 130px;
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

  .card {
    padding: 0.4rem;
    margin-top: 4.5rem;
  }
</style>

<div class="card">
  <h2>My Skills</h2>
  <p>
    I have spent a lot of my time working with React and Svelte on the front
    end, while on the backend the majority of my experience is using Nodejs. I
    also know Deno as I think it will only grow in popularity and I am always
    looking to get ahead of the raging tide that is new things in web
    development.
  </p>

  <div class="container">
    <div class="skill svelte image" />
    <div class="skill deno" />
    <div class="skill node" />
    <div class="skill react" />
  </div>
</div>
