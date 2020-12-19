<script>
</script>

<style>
  h2 {
    margin-top: 0;
    text-align: center;
  }

  .project-container p {
    margin: auto;
    text-align: center;
    font-size: 1.1rem;
    font-weight: 800;
  }

  .container {
    margin-top: 1.75rem;
    max-width: 1200px;
    margin: auto;
  }

  .list-container {
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
    background-size: 100%;
    background-repeat: no-repeat;
    width: 100%;
    height: 10rem;
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

  .description {
    display: none;
    background-color: #333;
    height: fit-content;
  }

  @media only screen and (min-width: 600px) {
    .list-container {
      /* display: grid;
      grid-template-columns: repeat(2, 1fr); */
    }
    .project-container .name {
      display: none;
    }
    .project-container .description {
      display: inline-block;
    }
    .project-container {
      display: grid;
      grid-template-columns: 1fr 1fr;
    }
    .noot {
      height: 100%;
      background-size: auto;
    }
  }
</style>

<div class="container">
  <h2>Projects</h2>
  <div class="list-container">
    <div class="project-container">
      <!-- <img src="../assets/project-thumbnails/noot-wear.png" alt="" /> -->
      <div class="noot-wear" />
      <p class="name">Noot Wear (E-Commerce)</p>
      <p class="description">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro unde hic
        animi accusantium laborum laboriosam accusamus. Id, nostrum quia ullam
        perferendis molestiae harum! Nesciunt doloribus, suscipit velit itaque
        aspernatur reprehenderit natus veniam id eligendi eum, quibusdam
        voluptates? Nisi ex numquam, dolorum harum delectus aut non natus
        placeat tempore laboriosam nam.
      </p>
    </div>
    <div class="project-container">
      <p class="description">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro unde hic
        animi accusantium laborum laboriosam accusamus. Id, nostrum quia ullam
        perferendis molestiae harum! Nesciunt doloribus, suscipit velit itaque
        aspernatur reprehenderit natus veniam id eligendi eum, quibusdam
        voluptates? Nisi ex numquam, dolorum harum delectus aut non natus
        placeat tempore laboriosam nam.
      </p>
      <div class="monster-rolodex" />
      <p class="name">Monsters Rolodex (React)</p>
    </div>
    <div class="project-container">
      <div class="popular-nerd" />
      <p class="name">PacMan (React Game)</p>
      <p class="description">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Porro unde hic
        animi accusantium laborum laboriosam accusamus. Id, nostrum quia ullam
        perferendis molestiae harum! Nesciunt doloribus, suscipit velit itaque
        aspernatur reprehenderit natus veniam id eligendi eum, quibusdam
        voluptates? Nisi ex numquam, dolorum harum delectus aut non natus
        placeat tempore laboriosam nam.
      </p>
    </div>
  </div>
</div>
