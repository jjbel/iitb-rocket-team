<script>
  import ChevronsRight from 'lucide-svelte/icons/chevrons-right';
  import ChevronsUp from 'lucide-svelte/icons/chevrons-up';

  import { base } from '$app/paths';
</script>

<!-- TODO later make a guide for these base url fixes for github pages -->
<div id="intro" style="--bg-image-url: url('{base}/agastya-5817.jpg');">
  <div id="title">
    <h2>Reaching New</h2>
    <h2>Frontiers in</h2>
    <h1 id="h1-glow">High Powered</h1>
    <h1>Rocketry</h1>
  </div>

  <a href="{base}/contact" id="contact">
    Contact Us <ChevronsRight id="contact-chevrons" color="var(--bg)" />
  </a>

  <div id="caption">
    <div id="caption_chevrons_mobile">
      <ChevronsUp size="2rem" color="var(--fg)" />
    </div>

    <div>Agastya leaving a trail of smoke and fire in its wake.</div>

    <div id="caption_chevrons_desktop">
      <ChevronsRight size="2rem" color="var(--fg)" />
    </div>
  </div>
</div>

<style>
  #intro {
    padding: 10vh 10vw 0 10vw;

    background-image:
      linear-gradient(to right, var(--bg) 45%, transparent 80%),
      var(--bg-image-url);

    background-size: cover;
    background-position:
      0 0,
      30vw 0vh;

    height: calc(100vh - var(--navbar-height));

    border-bottom: 1.5px solid var(--fg-gray);

    position: relative;
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

  #caption {
    position: absolute;
    left: 45%;
    bottom: 1rem;
    transform: translateX(-100%);

    width: 15rem;

    display: flex;
    align-items: center;
    gap: 1rem;

    background-color: rgba(155, 155, 155, 0.13);
    padding: 0.8rem;
    border-radius: 0.6rem;
    border: 0.1rem solid var(--fg-gray);
  }

  #caption_chevrons_mobile {
    display: none;
  }

  #caption_chevrons_desktop {
    display: block;
  }

  @media (max-aspect-ratio: 1) {
    #intro {
      background-image:
        linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
        var(--bg-image-url);

      background-size: cover;
      background-position:
        0 0,
        50% 0vh;
    }

    #caption {
      width: 20rem;
      color: rgb(212, 212, 212);
      left: 10%;
      bottom: 5rem;
      transform: none;
    }

    #caption_chevrons_mobile {
      display: block;
    }

    #caption_chevrons_desktop {
      display: none;
    }
  }
</style>
