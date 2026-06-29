<script>
  import { navLinks, APPLY_URL } from '../data/content.js';

  let { scrolled = $bindable(false) } = $props();

  function handleScroll() {
    scrolled = window.scrollY > 40;
  }
</script>

<svelte:window onscroll={handleScroll} />

<header class="header" class:header--scrolled={scrolled}>
  <div class="container header__inner">
    <a href="/" class="header__logo" aria-label="Skills4Her — inicio">
      <span class="header__logo-mark">S4</span>
      <span class="header__logo-text">Skills<span class="header__logo-accent">4</span>Her</span>
    </a>

    <nav class="header__nav" aria-label="Navegación principal">
      {#each navLinks as link}
        <a href={link.href}>{link.label}</a>
      {/each}
    </nav>

    <a href={APPLY_URL} class="btn btn--primary header__cta" target="_blank" rel="noopener noreferrer">
      Postularme
    </a>
  </div>
</header>

<style>
  .header {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 100;
    height: var(--header-height);
    display: flex;
    align-items: center;
    transition: background 0.3s, box-shadow 0.3s, backdrop-filter 0.3s;
  }

  .header--scrolled {
    background: rgba(250, 248, 252, 0.92);
    backdrop-filter: blur(12px);
    box-shadow: 0 1px 0 var(--color-border);
  }

  .header__inner {
    display: flex;
    align-items: center;
    gap: 2rem;
  }

  .header__logo {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    text-decoration: none;
    color: var(--color-text);
    font-family: var(--font-display);
    font-weight: 700;
    font-size: 1.2rem;
    flex-shrink: 0;
  }

  .header__logo:hover {
    text-decoration: none;
  }

  .header__logo-mark {
    background: linear-gradient(135deg, var(--color-primary), var(--color-accent));
    color: white;
    width: 2rem;
    height: 2rem;
    border-radius: 8px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 0.75rem;
  }

  .header__logo-accent {
    color: var(--color-accent);
  }

  .header__nav {
    display: flex;
    gap: 1.5rem;
    margin-left: auto;
  }

  .header__nav a {
    font-size: 0.9rem;
    font-weight: 500;
    color: var(--color-text-muted);
    text-decoration: none;
    transition: color 0.2s;
  }

  .header__nav a:hover {
    color: var(--color-primary);
    text-decoration: none;
  }

  .header__cta {
    padding: 0.625rem 1.25rem;
    font-size: 0.9rem;
    flex-shrink: 0;
  }

  @media (max-width: 900px) {
    .header__nav {
      display: none;
    }
  }

  @media (max-width: 480px) {
    .header__cta {
      padding: 0.5rem 1rem;
      font-size: 0.85rem;
    }

    .header__logo-text {
      display: none;
    }
  }
</style>
