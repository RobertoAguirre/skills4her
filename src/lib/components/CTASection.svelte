<script>
  import { APPLY_URL } from '../data/content.js';
</script>

<section class="cta">
  <div class="container cta__inner">
    <h2>Postúlate a Skills4Her</h2>
    <p>
      Da el primer paso para fortalecer tus habilidades, tu confianza y tus oportunidades en el
      mundo digital.
    </p>
    <p class="cta__urgency">
      Convocatoria abierta hasta el <strong>17 de julio de 2026</strong>. Solo
      <strong>50 lugares</strong> disponibles.
    </p>
    <a href={APPLY_URL} class="btn btn--primary cta__btn" target="_blank" rel="noopener noreferrer">
      Postularme ahora
    </a>
  </div>
</section>

<style>
  .cta {
    background: linear-gradient(135deg, var(--color-primary) 0%, #9333ea 50%, var(--color-accent) 100%);
    padding-block: 4rem;
    text-align: center;
    color: white;
  }

  .cta__inner {
    max-width: 600px;
  }

  .cta h2 {
    font-size: clamp(1.75rem, 4vw, 2.25rem);
    margin-bottom: 1rem;
  }

  .cta p {
    font-size: 1.05rem;
    line-height: 1.7;
    opacity: 0.92;
    margin-bottom: 0.75rem;
  }

  .cta__urgency {
    font-size: 0.95rem;
    margin-bottom: 2rem !important;
  }

  .cta__btn {
    background: white;
    color: var(--color-primary);
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.2);
    font-size: 1.05rem;
    padding: 1rem 2.5rem;
  }

  .cta__btn:hover {
    background: #faf8fc;
    box-shadow: 0 8px 28px rgba(0, 0, 0, 0.25);
  }
</style>
