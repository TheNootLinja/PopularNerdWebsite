<script>
</script>

<style>
  .container {
    width: 90%;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    margin: auto;
    gap: 2rem;
  }

  .project-card {
    /* background-color: gray; */
    height: 85%;
    width: 90%;
    text-align: center;
    margin: auto;
  }

  .project-container {
    background-color: rgb(218, 218, 218);
    padding: 0px 5px;
    height: 11rem;
  }

  .noot-wear {
    background-image: url("../assets/project-thumbnails/noot-wear.png");
    background-position: center;
    background-size: contain;
    background-repeat: no-repeat;
  }
  .popular-nerd {
    background-image: url("../assets/project-thumbnails/popularnerd.png");
    background-position: center;
    background-size: contain;
    background-repeat: no-repeat;
  }
  .monster-rolodex {
    background-image: url("../assets/project-thumbnails/monster-rolodex.png");
    background-position: center;
    background-size: contain;
    background-repeat: no-repeat;
  }
  h3 {
    background-color: rgba(155, 155, 155, 0.7);
    width: 100%;
    text-align: center;
    margin-bottom: 5px;
    margin-top: 5px;
    font-size: 1.5rem;
  }

  @media only screen and (max-width: 600px) {
    .container {
      display: block;
    }
    .project-container {
      margin-bottom: 10px;
      padding-bottom: 10px;
    }
  }
</style>

<h2>Projects</h2>
<div class="container">
  <div class="project-container">
    <div class="project-card noot-wear" />
    <h3>Noot-Wear</h3>
  </div>
  <div class="project-container">
    <div class="project-card popular-nerd" />
    <h3>Popular Nerd Site</h3>
  </div>
  <div class="project-container">
    <div class="project-card monster-rolodex" />
    <h3>Monster Rolodex</h3>
  </div>
  <div class="project-container">
    <div class="project-card noot-wear" />
    <h3>RealTime Chat App</h3>
  </div>
  <div class="project-container">
    <div class="project-card noot-wear" />
    <h3>Tinder Clone</h3>
  </div>
  <div class="project-container">
    <div class="project-card noot-wear" />
    <h3>PacMan</h3>
  </div>
</div>
