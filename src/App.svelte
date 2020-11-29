<script>
  import Header from "./UI/Header.svelte";
  import ProjectGrid from "./ProjectGrid.svelte";
  import ContactInformation from "./ContactInformation.svelte";
</script>

<style>
  main {
    color: #1b2d45;
    text-align: center;
    margin: 7rem auto;
  }

  h1 {
    color: rgb(90, 90, 90);
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
    margin: auto;
    margin-bottom: 5rem;
    max-width: 700px;
  }

  h2 {
    padding-left: 5rem;
  }

  .about-me {
    max-width: 1000px;
    margin: auto;
    background: rgb(238, 238, 238);
    padding: 3.5rem 1rem;
    box-shadow: 3px 3px 10px 0px #ccc;
  }

  span {
    color: #1b2d45;
  }

  h1 {
    animation: fadeInAnimation ease 6s;
    animation-iteration-count: 1;
    animation-fill-mode: forwards;
  }

  @keyframes fadeInAnimation {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }
</style>

<Header />
<main>
  <h1>My name is <span>Nicholas Peters</span></h1>
  <!-- TODO: Want to put the about me section inside of a card -->
  <p class="about-me" id="aboutme">
    And I am a full-stack developer from Michigan with a love for coffee (or
    maybe just caffeine). I perform web development under the company name
    Popular Nerd. My educational background is in IT Support and am a self taught
    programmer with experience in python, c++, and c#, but most of all, web
    development. when I started teaching myself web development I really found
    what I had a passion for. The feeling of getting to see something come to
    life piece by piece as quickly as I am able to put it together in my mind.
    Not only am I able to participate in setting up how code will function
    behind the scenes, but I also get to design how I think it should look on
    the front-end.
  </p>
</main>
<!-- This will be handled by the ProjectGrid component -->
<ProjectGrid />

<ContactInformation />
<!-- Possibly a contact info component -->
<h2>Possibly a footer at this point in the page</h2>
<!--  -->
