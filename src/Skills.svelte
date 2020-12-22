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
    grid-template-columns: 1fr 1fr 1fr;
    width: 90%;
    justify-content: space-around;
    margin: auto;
    gap: 5px;
  }

  .skill {
    /* background-color: lightgrey; */
    width: 100px;
    height: 100px;
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
  }

  .node {
    background-image: url("../assets/skill-logos/nodejs.svg");
  }

  .graphql {
    background-image: url("../assets/skill-logos/graphql.svg.png");
  }

  .html5 {
    background-image: url("../assets/skill-logos/HTML5.svg.png");
  }

  @media only screen and (min-width: 700px) {
    .grid-container {
      justify-content: center;
      width: 50%;
    }
    .skill {
      margin-top: 20px;
      width: 125px;
      height: 125px;
    }
  }
  @media only screen and (min-width: 1000px) {
    .container {
      display: grid;
      grid-template-columns: 1fr 1fr;
    }
    .skilldescription {
      margin: auto auto;
    }
  }
  @media only screen and (min-width: 1200px) {
    .skill {
      margin-top: 20px;
    }
  }
</style>

<div class="container">
  <div class="skilldescription">
    <h2>My Skills</h2>
    <p>
      In my time learning web development I have had a chance to use and
      experiment with a lot of different technologies. While I have general
      experience in many of these technologies, the bulk of my experience on the
      front-end is with React and Svelte. I feel like these 2 frameworks were a
      good pair to spend my time on as they compliment each other in what they
      are most useful for building, and the amount of knowledge and concepts
      that carries from one to the other. On back-end development I started with
      using Nodejs as I already had JavaScript experience, but more recently I
      have started using Deno as I think that it will only continue to grow in
      use as time moves forward.
    </p>
  </div>

  <div class="grid-container">
    <div class="skill svelte" />
    <div class="skill deno" />
    <div class="skill react" />
    <div class="skill node" />
    <div class="skill html5" />
    <div class="skill graphql" />
  </div>
</div>
