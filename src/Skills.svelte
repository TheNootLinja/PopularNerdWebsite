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
    margin: auto;
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
    margin-right: unset;
  }

  .react {
    background-image: url("../assets/skill-logos/react2.png");
    margin-left: unset;
  }

  .deno {
    background-image: url("../assets/skill-logos/Deno.svg.png");
    background-color: white;
    border-radius: 100%;
    margin-left: unset;
  }

  .node {
    background-image: url("../assets/skill-logos/nodejs.svg");
    margin-right: unset;
  }

  .svelte {
    background-image: url("../assets/skill-logos/Svelte_Logo.svg.png");
  }

  .svelte {
    background-image: url("../assets/skill-logos/Svelte_Logo.svg.png");
  }

  @media only screen and (min-width: 700px) {
    .grid-container {
      justify-content: center;
      width: 50%;
    }
    .skill {
      margin-top: 20px;
      width: 150px;
      height: 150px;
    }
  }
  @media only screen and (min-width: 1200px) {
    .skill {
      margin-top: 20px;
      width: 200px;
      height: 200px;
    }
  }
  @media only screen and (min-width: 2560px) {
    .skill {
      margin-top: 20px;
      width: 300px;
      height: 300px;
    }
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
