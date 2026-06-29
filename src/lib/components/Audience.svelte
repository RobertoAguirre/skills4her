<script>
  import { audienceSignals } from '../data/content.js';
</script>

<section class="section">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Convocatoria</span>
      <h2>¿Para quién es este programa?</h2>
      <p class="section__lead">
        Esta convocatoria está dirigida a mujeres de 18 años en adelante, incluyendo mujeres
        cisgénero, mujeres trans y personas que se identifiquen como mujeres, que residan
        permanentemente en Ciudad Juárez, Chihuahua.
      </p>
    </header>

    <div class="audience__box">
      <h3>Este programa puede ser para ti si:</h3>
      <ul class="check-list">
        {#each audienceSignals as signal}
          <li>{signal}</li>
        {/each}
      </ul>
    </div>
  </div>
</section>

<style>
  .audience__box {
    background: var(--color-surface);
    border: 1px solid var(--color-border);
    border-radius: var(--radius-lg);
    padding: 2rem;
    box-shadow: var(--shadow);
    max-width: 720px;
  }

  .audience__box h3 {
    font-size: 1.125rem;
    margin-bottom: 1.25rem;
    color: var(--color-primary);
  }
</style>
