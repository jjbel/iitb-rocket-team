<script>
  import Intro from './home/Intro.svelte';

  import Achievements from './home/Achievements.svelte';
  import Rockets from './home/Rockets.svelte';
  import Tech from './home/Tech.svelte';
  import Testimonials from './home/Testimonials.svelte';
</script>

<Intro />

<div id="info">
  <h2>
    <span
      class="emphasis"
      style="--gradient-from: #ffe312; --gradient-to: #f68c14;">Awards</span
    > - testament to our excellence
  </h2>
  <Achievements />

  <h2>
    Meet the <span
      class="emphasis"
      style="--gradient-from: #86d1ff; --gradient-to: #0638ff;"
      >Rocket Family</span
    >
  </h2>
  <Rockets />

  <h2>
    Feat. the <span
      class="emphasis"
      style="--gradient-from: #ff2066; --gradient-to: #ff5618;">Hottest</span
    > Tech
  </h2>
  <Tech />
  
  <h2>
    Testimonials
  </h2>
  <Testimonials />
</div>

<style>
  /* @import url('https://fonts.googleapis.com/css2?family=Yellowtail&display=swap'); */

  #info {
    padding: 0vh 10% 0vh 10%;
    font-size: 1.2rem;
  }

  h2 {
    font-size: 3.2rem;
    margin-top: 2.5rem;
    margin-bottom: 0.2rem;
  }

  .emphasis {
    font-family: 'Yellowtail', serif;
    font-size: 4.5rem;
    padding-right: 1.1rem;

    background: linear-gradient(
      to right,
      var(--gradient-from),
      var(--gradient-to)
    );

    background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  @media (max-aspect-ratio: 1) {
    h2 {
      font-size: 1.9rem;
      margin-top: 3.5rem;
      margin-bottom: 1rem;
    }

    .emphasis {
      font-size: 2.5rem;
    }
  }
</style>
