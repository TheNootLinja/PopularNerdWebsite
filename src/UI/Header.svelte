<script>
</script>

<style>
  /* header {
    color: white;
    position: fixed;
    left: 0;
    top: 0;
    width: 100%;
    height: 3rem;
    background-color: #333;
    box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
    display: flex;
    justify-content: space-between;
    align-items: center;
  } */

  /* header nav a {
    color: white;
    text-decoration: none;
    border-bottom: solid 2px #00ebc7;
  } */

  header nav a + a {
    margin-left: 10px;
  }

  .last {
    margin-right: 2rem;
  }

  .fake-logo {
    font-size: 120%;
    margin: 0;
    margin-left: 2rem;
    padding-right: 6px;
  }

  .hb {
    width: 35px;
    height: 5px;
    background-color: #00ebc7;
    margin: 6px 20px;
    display: none;
  }

  .hb-container {
    display: none;
    height: 35px;
    width: fit-content;
  }

  @media only screen and (max-width: 500px) {
    a {
      display: none;
    }
    .hb {
      display: block;
    }
    .hb-container {
      display: block;
    }
  }
</style>

<header>
  <h1 class="fake-logo">Nicholas Peters</h1>
  <nav>
    <a href="#aboutme">About</a>
    <a href="#projectgrid">Projects</a>
    <a href="#contact" class="last">Contact</a>
  </nav>
</header>
