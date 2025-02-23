<script>
</script>

<div id="intro">
  <!-- <img src={agastya_hero} alt="Agastya Launch" /> -->

  <h2>Reaching New</h2>
  <h2>Frontiers in</h2>
  <h1 id="h1-glow">High Powered</h1>
  <h1>Rocketry</h1>

  <a href="/contact" id="contact"> Contact Us </a>
</div>

<div id="tech">
  <h2>Feat. the <span id="hottest">Hottest</span> Tech</h2>
  <p>
    <strong>FLYTE</strong> - Our latest flight computer
    <a href="">Check it out</a>
  </p>
</div>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Yellowtail&display=swap');

  #intro {
    padding: 8% 10% 0 10%;

    background-image:
      linear-gradient(to right, rgb(0, 0, 0) 50%, rgba(0, 0, 0, 0) 70%),
      url('/agastya-5815.jpg');

    background-size: cover;
    background-position:
      0 0,
      30vw -10vh;

    height: calc(100vh - var(--navbar-height));
  }

  #intro h2 {
    font-size: 3rem;
  }

  #intro h1 {
    font-size: 5rem;
  }

  #h1-glow {
    text-shadow: rgba(255, 255, 255, 0.76) 0 0 0.7rem;
  }

  #contact {
    display: inline-block;
    background-color: white;
    color: black;
    border: none;
    font-weight: 600;

    font-size: 1.6rem;
    border-radius: 0.4rem;
    padding: 1rem;
    margin-top: 5vh;
  }

  #tech {
    padding: 2% 10% 0 10%;
  }

  #tech h2 {
    font-size: 3rem;
    vertical-align: middle;
  }

  #hottest {
    font-family: 'Yellowtail', serif;
    font-size: 4.2rem;
    padding-right: 0.9rem;

    background: linear-gradient(to right, #ff237b, #ff3b19);
    background-clip: text;
    -webkit-text-fill-color: transparent;
  }
</style>
