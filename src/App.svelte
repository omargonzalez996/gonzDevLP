<script>
  import Navbar from "./components/Navbar.svelte";
</script>

<video autoplay muted loop id="back-vid">
  <source src="/back2.mp4" type="video/mp4" />
</video>

<div class="App">
  <div class="App-container">
    <div class="App-content">
      <div class="App-title">
        <h1>GonzDev</h1>
        <p>Omar González</p>
      </div>
      <figure>
        <img class="logo-pic" src="/tall-logo.png" alt="gonzDev_Logo" />
      </figure>
    </div>
    <div class="navbar-container">
      <Navbar />
    </div>
  </div>
</div>

<style>
  @font-face {
    font-family: Pacifico;
    src: url("https://fonts.googleapis.com/css?family=Pacifico");
  }
  :global(*) {
    box-sizing: border-box;
  }

  :global(body) {
    font-family: "Pacifico";
    margin: 0;
    padding: 0;
    color: white;
    overflow: hidden;
  }
  #back-vid {
    filter: blur(10px);
    position: fixed;
    right: 0;
    bottom: 0;
    top: 0px;
    left: 0px;
    min-width: 100%;
    min-height: 100%;
    border: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
  }
  .App {
    background: rgba(15, 62, 116, 0.5);
    color: #fff;
    position: absolute;
    bottom: 0;
    top: 0;
    width: 100%;
    padding: 1em;
    user-select: none;
    -moz-user-select: none;
    -webkit-user-drag: none;
    -webkit-user-select: none;
    -ms-user-select: none;
  }
  .App-container {
    display: grid;
    grid-template-columns: minmax(auto, 1280px);
    justify-content: center;
    align-items: center;
  }
  .App-content {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 30px;
  }
  .logo-pic {
    filter: invert(1);
    width: 70%;
    height: 120%;
  }
  h1 {
    font-size: 75px;
    margin: 0;
    padding: 0;
    letter-spacing: 2px;
    text-shadow: 6px 6px 0px rgba(0, 0, 0, 0.2);
  }
  p {
    font-size: 40px;
    margin: 0;
    padding: 0;
    letter-spacing: 1.2px;
    text-shadow: 3px 3px 0px rgba(0, 0, 0, 0.2);
  }
  figure {
    margin: 0;
    padding: 0;
    text-align: right;
  }
  @media (max-width: 534px) {
    .App-title {
      text-align: center;
    }
    h1 {
      font-size: 50px;
    }
    p {
      font-size: 25px;
    }
    .App-content {
      margin-top: 70px;
      display: block;
    }
    .logo-pic {
      margin-top: 30px;
      width: 40%;
    }
    figure {
      text-align: center;
    }
  }
</style>
