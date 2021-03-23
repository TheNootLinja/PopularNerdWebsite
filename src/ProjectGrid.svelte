<script>
</script>

<style>
  h2 {
    margin-top: 0;
    text-align: center;
  }
  h4 {
    padding-top: 0;
    margin-top: 0;
  }
  ul {
    text-align: center;
    padding: 0;
    margin-top: 0;
  }

  li {
    list-style: none;
  }

  a {
    color: white;
  }
  p {
    margin-bottom: 0;
  }
  .name {
    margin: auto;
    text-align: center;
    font-size: 1.1rem;
    font-weight: 800;
  }

  .container {
    margin: auto;
    margin-top: 1.75rem;
    max-width: 1200px;
  }

  .list-container {
    width: 90%;
    margin: auto;
  }

  .project-container {
    /* background-color: rgb(218, 218, 218); */
    margin-bottom: 15px;
    /* width: fit-content; */
  }

  .website {
    margin-top: 5rem;
  }

  .noot-wear {
    background-image: url("../assets/project-thumbnails/noot-wear.png");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
    height: 15rem;
  }
  .whats-on {
    background-image: url("../assets/project-thumbnails/whatson.png");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
    height: 15rem;
  }

  .popular-nerd {
    background-image: url("../assets/project-thumbnails/popularnerd.png");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    height: 15rem;
    width: 100%;
  }
  .spacer {
    background-color: rgba(0, 0, 0, 0);
  }

  .projectdesccont {
    background-color: #333;
    display: none;
    position: relative;
    text-align: center;
  }
  .project-link {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    padding-left: auto;
    margin-bottom: 10px;
  }

  @media only screen and (min-width: 600px) {
    p {
      text-align: center;
    }
    .project-container .name {
      display: none;
    }
    .project-container {
      display: grid;
      grid-template-columns: 30fr 1fr 30fr;
    }
    .projectdesccont {
      display: block;
    }
  }
</style>

<div class="container">
  <h2>Projects</h2>
  <div class="list-container">
    <div class="project-container">
      <!-- Project picture #1 -->
      <a href="/">
        <div class="noot-wear" />
      </a>
      <p class="name">Noot Wear (E-Commerce)</p>
      <div class="spacer" />
      <div class="projectdesccont">
        <h4>Noot-Wear</h4>
        <p>An ecommerce site for a fictitious brand, noot-wear.</p>
        <!-- Project link #1 -->
        <a class="project-link" target="blank" href="/">See The Live Site</a>
      </div>
    </div>
    <div class="project-container">
      <div class="projectdesccont">
        <h4>What's On?</h4>
        <p>
          This is one of the first projects I did when learning React. The app
          hits an api, shows some use of components
        </p>
        <!-- Project link #2 -->
        <a class="project-link" href="/">See The Live Site</a>
      </div>
      <div class="spacer" />
      <!-- Project picture #2 -->
      <a target="blank" href="https://compassionate-shaw-0e3725.netlify.app/">
        <div class="whats-on" />
      </a>
      <p class="name">Monsters Rolodex (React)</p>
    </div>
    <div class="project-container">
      <!-- Project Picture #3 -->
      <a href="/">
        <div class="popular-nerd" />
      </a>
      <p class="name">PacMan (Javascript Game)</p>
      <div class="spacer" />
      <div class="projectdesccont">
        <h4>Meetups</h4>
        <p>
          This is one of the first projects I did when learning React. The app
          hits an api, shows some use of components
        </p>
        <!-- Project link #3 -->
        <a class="project-link" href="/">See The Live Site</a>
      </div>
    </div>
  </div>
</div>
