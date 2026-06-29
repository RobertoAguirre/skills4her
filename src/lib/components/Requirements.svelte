<script>
  import { requirements } from '../data/content.js';
</script>

<section id="requisitos" class="section section--dark">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Postulación</span>
      <h2>Requisitos para postular</h2>
      <p class="section__lead">
        Para participar deberás cumplir con lo siguiente:
      </p>
    </header>

    <ul class="check-list requirements__list">
      {#each requirements as req}
        <li>{req}</li>
      {/each}
    </ul>
  </div>
</section>

<style>
  .requirements__list {
    max-width: 720px;
    grid-template-columns: 1fr;
  }
</style>
