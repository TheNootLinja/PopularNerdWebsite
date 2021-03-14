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
    /* background-image: url("../assets/pictures/nppicture.jpg");
    background-position: center;
    background-size: contain;
    background-repeat: no-repeat; */
  }

  h1 {
    color: rgb(90, 90, 90);
    text-transform: uppercase;
    font-size: 3em;
    font-weight: 100;
    margin: auto;
    margin-bottom: 0.25rem;
    /* max-width: 700px; */
    text-align: center;
  }

  h2 {
    text-align: center;
    margin-top: 0;
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
    width: 100%;
    height: 310px;
    margin: auto;
  }
  .container {
    max-width: 1500px;
    margin: auto;
  }

  .img-container {
    text-align: center;
    overflow: hidden;
    width: 100%;
  }

  .grid {
    display: block;
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
      width: 100%;
      height: 600px;
    }
    h1 {
      width: 500px;
      margin-bottom: 1rem;
    }
    .img-container {
      overflow: hidden;
      height: 250px;
    }
    img {
      padding-bottom: 30px;
    }
  }
  @media only screen and (min-width: 1000px) {
    h2 {
      margin-top: 0;
    }
    .grid {
      display: grid;
    }
    .twocol {
      grid-template-columns: 2fr 0fr 3fr;
    }
    img {
      width: 700px;
      margin: auto auto;
    }
    .aboutme {
      margin: auto auto;
    }
    .img-container {
      height: 400px;
      width: 95%;
      margin: auto;
    }
  }
  @media only screen and (min-width: 1550px) {
    h1 {
      margin-top: 3rem;
      margin-bottom: 5rem;
    }
    .img-container {
      text-align: right;
    }
  }
</style>

<Header on:openmenu={openMenu} hbOpen={mobMenuOpen} />
{#if mobMenuOpen}
  <PopUpMenu on:closemenu={openMenu} />
{/if}
<div class="container">
  <main>
    <h1>My name is <span>Nicholas Peters</span></h1>
    <div class="grid twocol">
      <div class="img-container">
        <img src="../assets/pictures/nppicture.jpg" alt="" />
      </div>
      <br id="aboutme" />
      <div class="aboutme">
        <h2>About Me</h2>
        <p>
          I am a full-stack developer from Michigan with a love for coffee, tech, 
          and did I mention coffee? I do freelance and contract web development 
          under the company name Popular Nerd over at popularnerd.tech. I have a 
          background in IT Support but I am a self taught programmer with experience 
          in python, c++, and c#, but most of all, the vast world of 
          <em><strong>web development</strong></em>. On top of all of that, I currently 
          build applications and solutions in the Microft Power Platform as a full time 
          job so I have experience with PowerApps, PowerBI, Power Automate, and other 
          parts of previously mentioned enviroment.
        </p>
      </div>
    </div>
  </main>
  <br id="skills" />
  <Skills />
  <br id="projectgrid" />
  <ProjectGrid />
  <br id="prevexp" />
  <PreviousExperience />
  <br id="contact" />
  <ContactInformation />
</div>
<Footer />
