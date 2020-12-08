<script>
  import Header from './UI/Header.svelte';
  import ProjectGrid from './ProjectGrid.svelte';
  import ContactInformation from './ContactInformation.svelte';

  let mobMenuOpen = false;
</script>

<style>
  main {
    color: #1b2d45;
    padding-top: 4rem;
    margin: auto;
  }

  h2 {
    text-align: center;
  }

  h1 {
    color: rgb(90, 90, 90);
    text-transform: uppercase;
    font-size: 3em;
    font-weight: 100;
    margin: auto;
    margin-bottom: 2rem;
    max-width: 700px;
    text-align: center;
  }

  .about-me {
    max-width: 100%;
    margin: auto;
    background: rgb(238, 238, 238);
    box-shadow: 3px 3px 10px 0px #ccc;
    padding: 1rem 0;
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

  span {
    color: #1b2d45;
    animation: fadeInAnimation ease 4s;
    animation-iteration-count: 1;
    animation-fill-mode: forwards;
  }

  img {
    width: 80%;
    border-radius: 200px;
    margin: auto;
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
  <div class="img-container">
    <img src="../assets/pictures/nppicture.jpg" alt="" />
  </div>
  <br id="aboutme" />
  <div class="about-me">
    <p>
      I am a full-stack developer from Michigan with a love for coffee. I do
      freelance and contract web development under the company name Popular
      Nerd. My educational background is in IT Support and am a self taught
      programmer with experience in python, c++, and c#, but most of all, the
      vast world of
      <em><strong>web development</strong></em>. when I started teaching myself
      web development I really found what I had a passion for. The feeling of
      getting to see something come to life piece by piece as quickly as I am
      able to put it together in my mind. Not only am I able to participate in
      setting up how code will function behind the scenes, but I also get to
      design how I think it should look on the front-end.
    </p>
  </div>
</main>
<br id="skillgrid" />
<div class="skills">
  <h2>Programming Skills</h2>
</div>
<br id="projectgrid" />
<!-- This will be handled by the ProjectGrid component -->
<ProjectGrid />
<br id="contact" />
<ContactInformation />
<!-- Possibly a contact info component -->
<h2>Possibly a footer at this point in the page</h2>
<!--  -->
