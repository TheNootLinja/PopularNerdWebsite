<script>
  import Header from "./UI/Header.svelte";
  import ProjectGrid from "./ProjectGrid.svelte";
  import ContactInformation from "./ContactInformation.svelte";
  import Skills from "./Skills.svelte";
  import Footer from "./UI/Footer.svelte";
  import PreviousExperience from "./PreviousExperience.svelte";
  import PopUpMenu from "./UI/PopUpMenu.svelte";

  let mobMenuOpen = false;

  function openMenu() {
    console.log("It works!");
    mobMenuOpen = !mobMenuOpen;
    console.log(mobMenuOpen);
  }
</script>

<style>
  main {
    padding-top: 4rem;
    margin: auto;
  }

  h1 {
    color: rgb(90, 90, 90);
    text-transform: uppercase;
    font-size: 3em;
    font-weight: 100;
    margin: auto;
    margin-bottom: 2rem;
    /* max-width: 700px; */
    text-align: center;
  }

  h2 {
    text-align: center;
  }

  p {
    text-align: center;
    width: 95%;
    max-width: 800px;
    margin: auto;
  }

  span {
    color: #90a9b7;
    animation: fadeInAnimation ease 4s;
    animation-iteration-count: 1;
    animation-fill-mode: forwards;
    font-size: 3rem;
  }

  img {
    width: 80%;
    border-radius: 100%;
    margin: auto;
  }

  .about-me {
    max-width: 100%;
    margin: auto;
    background: rgb(238, 238, 238);
    box-shadow: 3px 3px 10px 0px #ccc;
    padding: 0 0 1rem 0;
    margin-top: 2.5rem;
  }

  .about-me p {
    text-align: center;
    margin: auto;
  }

  .skills {
    height: 15rem;
  }

  .img-container {
    text-align: center;
  }

  .card {
    width: 95%;
    margin: auto;
    text-align: center;
    padding: 0.4rem;
    padding-top: 1.2rem;
  }

  @keyframes fadeInAnimation {
    0% {
      opacity: 0;
    }
    100% {
      opacity: 1;
    }
  }

  @media only screen and (min-width: 600px) {
    img {
      width: 300px;
    }
    h1 {
      width: 500px;
    }
  }
</style>

<Header on:openmenu={openMenu} hbOpen={mobMenuOpen} />
{#if mobMenuOpen}
  <PopUpMenu on:closemenu={openMenu} />
{/if}
<main>
  <h1>My name is <span>Nicholas Peters</span></h1>
  <!-- TODO: Want to put the about me section inside of a card -->
  <div class="img-container">
    <img src="../assets/pictures/nppicture.jpg" alt="" />
  </div>
  <br id="aboutme" />
  <h2>About Me</h2>
  <p>
    I am a full-stack developer from Michigan with a love for coffee, tech, and
    did I mention coffee? I do freelance and contract web development under the
    company name Popular Nerd over at popularnerd.tech. My educational
    background is in IT Support and am a self taught programmer with experience
    in python, c++, and c#, but most of all, the vast world of
    <em><strong>web development</strong></em>. when I started teaching myself
    web development I really found what I had a passion for. The feeling of
    getting to see something come to life piece by piece as quickly as I am able
    to put it together in my mind. Not only am I able to participate in setting
    up how code will function behind the scenes, but I also get to design how I
    think it should look on the front-end.
  </p>
</main>
<br id="skills" />
<Skills />
<br id="prevexp" />
<PreviousExperience />
<br id="projectgrid" />
<!-- This will be handled by the ProjectGrid component -->
<ProjectGrid />
<br id="contact" />
<ContactInformation />
<Footer />
