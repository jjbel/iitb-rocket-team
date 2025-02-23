<script>
  // https://www.okupter.com/blog/deploy-sveltekit-website-to-github-pages
  import { base } from '$app/paths';

  import logo from '$lib/rtlogo1.png'

  const links = [
    ['/', 'Home'],
    ['/sponsor', 'Sponsor'],
    ['/sponsor', 'Team'],
    ['/sponsor', 'Rockets'],
    ['/sponsor', 'Contact']
  ];
</script>

<nav>
  <img src={logo} alt="IITB Rocket Team" />

  <div class="links">
    {#each links as link}
      <a href="{base}/{link[0]}">{link[1]}</a>
    {/each}
  </div>
</nav>

<style>
  nav {
    display: flex;
    /* background-color: rgb(98, 98, 98); */

    color: rgb(232, 232, 232);
    padding: 0 4rem;
    height: var(--navbar-height);
    justify-content: center;
  }

  img {
    height: 100%;
  }

  .links {
    display: flex;
    padding: 0.9rem 4rem;
    font-size: 1.4rem;
    gap: 3rem;
    justify-content: center;
    align-items: center;
  }
</style>
