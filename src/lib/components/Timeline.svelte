<script>
  import { timeline } from '../data/content.js';
</script>

<section id="fechas" class="section">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Calendario</span>
      <h2>Fechas importantes</h2>
    </header>

    <ol class="timeline">
      {#each timeline as item, i}
        <li class="timeline__item">
          <div class="timeline__marker" aria-hidden="true">
            <span class="timeline__dot"></span>
            {#if i < timeline.length - 1}
              <span class="timeline__line"></span>
            {/if}
          </div>
          <div class="timeline__content">
            <time class="timeline__date">{item.date}</time>
            <p class="timeline__event">{item.event}</p>
          </div>
        </li>
      {/each}
    </ol>
  </div>
</section>

<style>
  .timeline {
    list-style: none;
    max-width: 640px;
  }

  .timeline__item {
    display: flex;
    gap: 1.25rem;
  }

  .timeline__marker {
    display: flex;
    flex-direction: column;
    align-items: center;
    flex-shrink: 0;
    width: 1.25rem;
  }

  .timeline__dot {
    width: 12px;
    height: 12px;
    border-radius: 50%;
    background: linear-gradient(135deg, var(--color-primary), var(--color-accent));
    flex-shrink: 0;
    margin-top: 0.35rem;
  }

  .timeline__line {
    width: 2px;
    flex: 1;
    background: var(--color-border);
    margin-block: 0.25rem;
    min-height: 2rem;
  }

  .timeline__content {
    padding-bottom: 1.75rem;
  }

  .timeline__date {
    display: block;
    font-family: var(--font-display);
    font-size: 0.9rem;
    font-weight: 700;
    color: var(--color-primary);
    margin-bottom: 0.25rem;
  }

  .timeline__event {
    font-size: 1rem;
    color: var(--color-text);
  }
</style>
