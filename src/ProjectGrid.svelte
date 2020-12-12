<script>
</script>

<style>
  .project-container p {
    margin: auto;
    text-align: center;
    font-size: 1.1rem;
    font-weight: 800;
  }

  h2 {
    text-align: center;
  }

  h3 {
    background-color: rgba(155, 155, 155, 0.7);
    width: 100%;
    text-align: center;
    margin-bottom: 5px;
    margin-top: 5px;
    font-size: 1.5rem;
  }

  .container {
    width: 90%;
    margin: auto;
  }

  .project-container {
    background-color: rgb(218, 218, 218);
    margin-bottom: 15px;
    /* width: fit-content; */
  }

  .noot-wear {
    background-image: url("../assets/project-thumbnails/noot-wear.png");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    height: 10rem;
    width: 100%;
  }

  .popular-nerd {
    background-image: url("../assets/project-thumbnails/popularnerd.png");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    height: 10rem;
    width: 100%;
  }

  .monster-rolodex {
    background-image: url("../assets/project-thumbnails/monster-rolodex.png");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    height: 10rem;
    width: 100%;
  }

  @media only screen and (min-width: 600px) {
    .container {
      display: block;
    }
  }
</style>

<h2>Projects</h2>
<div class="container">
  <div class="project-container">
    <div class="noot-wear" />
    <p>Noot Wear (E-Commerce)</p>
  </div>
  <div class="project-container">
    <div class="monster-rolodex" />
    <p>Monsters Rolodex (React)</p>
  </div>
  <div class="project-container">
    <div class="popular-nerd" />
    <p>PacMan (React Game)</p>
  </div>
</div>
