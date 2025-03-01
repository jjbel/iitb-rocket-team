<script>
  import ChevronsRight from 'lucide-svelte/icons/chevrons-right';
  import { base } from '$app/paths';
</script>

<div id="intro">
  <div id="title">
    <h2>Reaching New</h2>
    <h2>Frontiers in</h2>
    <h1 id="h1-glow">High Powered</h1>
    <h1>Rocketry</h1>
  </div>

  <a href="{base}/contact" id="contact">
    Contact Us <ChevronsRight id="chevrons" color="var(--bg)" />
  </a>
</div>

<style>
  #intro {
    padding: 16vh 10vw 0 10vw;

    background-image:
      linear-gradient(to right, var(--bg) 50%, transparent 70%),
      url('/agastya-5817.jpg');

    background-size: cover;
    background-position:
      0 0,
      30vw 0vh;

    height: calc(100vh - var(--navbar-height));

    border-bottom: 1.5px solid var(--fg-gray);
  }

  /* on mobile, the bg image is dark, so use the light theme styling only on desktop */

  @media (min-aspect-ratio: 1) {
    :global(body.light) #title {
      background: linear-gradient(135deg, black, #0004ff);
      background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    :global(body.light) #h1-glow {
      text-shadow: none;
    }
  }

  #title {
    background: linear-gradient(135deg, white, #b1b4fc);
    background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  #h1-glow {
    text-shadow: rgba(232, 242, 255, 0.76) 0.1rem 0 0.7rem;
  }

  h2 {
    font-size: 3rem;
  }

  h1 {
    font-size: 5rem;
  }

  #contact {
    display: flex;
    width: fit-content;
    align-items: center;
    gap: 0.3rem;

    background-color: var(--fg);
    color: var(--bg);
    border: none;
    font-weight: 600;

    font-size: 1.6rem;
    border-radius: 0.4rem;
    padding: 1rem;
    margin-top: 8vh;
  }

  @media (max-aspect-ratio: 1) {
    #intro {
      background-image:
        linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
        url('/agastya-5817.jpg');

      background-size: cover;
      background-position:
        0 0,
        50% 0vh;
    }
  }
</style>
