<script>
  import { selectionSteps } from '../data/content.js';
</script>

<section class="section section--dark">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Selección</span>
      <h2>¿Cómo será el proceso de selección?</h2>
    </header>

    <ol class="selection__steps">
      {#each selectionSteps as step, i}
        <li class="selection__step">
          <span class="selection__num">{i + 1}</span>
          <span class="selection__text">{step}</span>
        </li>
      {/each}
    </ol>

    <div class="selection__note">
      <p>
        Se seleccionarán <strong>50 beneficiarias</strong> y <strong>15 mujeres</strong> en lista
        de espera.
      </p>
      <p>
        El cumplimiento de requisitos no garantiza la selección automática, ya que el cupo es
        limitado.
      </p>
    </div>
  </div>
</section>

<style>
  .selection__steps {
    list-style: none;
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
    gap: 1rem;
    margin-bottom: 2rem;
  }

  .selection__step {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 1.25rem;
    background: rgba(255, 255, 255, 0.05);
    border: 1px solid rgba(255, 255, 255, 0.1);
    border-radius: var(--radius);
  }

  .selection__num {
    flex-shrink: 0;
    width: 2rem;
    height: 2rem;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(135deg, var(--color-primary), var(--color-accent));
    border-radius: 50%;
    font-family: var(--font-display);
    font-size: 0.875rem;
    font-weight: 700;
  }

  .selection__text {
    font-size: 0.95rem;
    line-height: 1.5;
  }

  .selection__note {
    max-width: 640px;
    padding: 1.25rem 1.5rem;
    background: rgba(255, 255, 255, 0.05);
    border-radius: var(--radius);
    border-left: 4px solid var(--color-accent);
    display: flex;
    flex-direction: column;
    gap: 0.5rem;
    font-size: 0.95rem;
    color: #c4b8d8;
  }

  .selection__note strong {
    color: white;
  }
</style>
