<script>
  import { quickStats } from '../data/content.js';
</script>

<section class="stats" aria-label="Datos rápidos del programa">
  <div class="container">
    <ul class="stats__grid">
      {#each quickStats as stat}
        <li class="stats__item">
          <span class="stats__label">{stat.label}</span>
          <span class="stats__value">{stat.value}</span>
        </li>
      {/each}
    </ul>
  </div>
</section>

<style>
  .stats {
    background: var(--color-surface);
    border-bottom: 1px solid var(--color-border);
    padding-block: 2rem;
    margin-top: -1px;
  }

  .stats__grid {
    list-style: none;
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(130px, 1fr));
    gap: 1.5rem;
  }

  .stats__item {
    text-align: center;
    padding: 0.5rem;
  }

  .stats__label {
    display: block;
    font-size: 0.75rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.06em;
    color: var(--color-text-muted);
    margin-bottom: 0.35rem;
  }

  .stats__value {
    display: block;
    font-family: var(--font-display);
    font-size: 1.1rem;
    font-weight: 700;
    color: var(--color-primary);
  }
</style>
