<script>
  // https://www.okupter.com/blog/deploy-sveltekit-website-to-github-pages
  import { base } from '$app/paths';
  import logo from '$lib/rtlogo1.png';
  import ThemeToggle from './ThemeToggle.svelte';

  const links = [
    ['', 'Home'],
    ['sponsor', 'Sponsor'],
    ['sponsor', 'Team'],
    ['sponsor', 'Rockets'],
    ['sponsor', 'Contact']
  ];
</script>

<nav>
  <img src={logo} alt="IITB Rocket Team" />

  <div id="links">
    {#each links as link}
      <a href="{base}/{link[0]}">{link[1]}</a>
    {/each}
  </div>

  <ThemeToggle />
</nav>

<style>
  nav {
    display: flex;
    background-color: var(--bg);

    padding: 0 4rem;
    height: var(--navbar-height);
    justify-content: center;
    align-items: center;
  }

  img {
    height: 100%;
  }

  #links {
    display: flex;
    padding: 0.9rem 4rem;
    font-size: 1.4rem;
    gap: 3rem;
    justify-content: center;
    align-items: center;
  }

  a {
    color: var(--fg);
  }

  @media (max-aspect-ratio: 1) {
    #links {
      display: none;
      /* TODO */
    }
  }
</style>
