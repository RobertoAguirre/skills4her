<script>
  import { benefits } from '../data/content.js';
</script>

<section class="section section--alt">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Beca completa</span>
      <h2>Beneficios de participar</h2>
      <p class="section__lead">
        Las mujeres seleccionadas recibirán una beca del <strong>100%</strong>. La beca incluye:
      </p>
    </header>

    <ul class="check-list benefits__list">
      {#each benefits as benefit}
        <li>{benefit}</li>
      {/each}
    </ul>
  </div>
</section>

<style>
  .benefits__list {
    max-width: 720px;
    grid-template-columns: 1fr;
  }

  .section__lead strong {
    color: var(--color-accent);
  }
</style>
