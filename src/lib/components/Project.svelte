<section class="section">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Proyecto final</span>
      <h2>Proyecto final y constancias</h2>
    </header>

    <div class="project__grid">
      <div class="project__main">
        <p>
          Durante el programa desarrollarás un <strong>proyecto tecnológico aplicado</strong>, de
          manera individual o en equipo de máximo 3 personas, utilizando herramientas de
          vibecoding para crear soluciones reales.
        </p>
        <p>
          Al cierre del programa se presentarán los <strong>15 mejores proyectos</strong>.
        </p>
      </div>

      <aside class="project__certs">
        <h3>Constancias al acreditar</h3>
        <ul class="check-list">
          <li>Constancia emitida por Democratizamos la Innovación A.C.</li>
          <li>Constancia con valor curricular emitida por CENALTEC.</li>
        </ul>
      </aside>
    </div>
  </div>
</section>

<style>
  .project__grid {
    display: grid;
    grid-template-columns: 1fr 340px;
    gap: 2rem;
    align-items: start;
  }

  .project__main {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    font-size: 1.05rem;
    color: var(--color-text-muted);
    line-height: 1.75;
  }

  .project__main strong {
    color: var(--color-text);
  }

  .project__certs {
    background: linear-gradient(135deg, var(--color-dark) 0%, var(--color-dark-soft) 100%);
    color: #f0eaf8;
    border-radius: var(--radius-lg);
    padding: 1.75rem;
  }

  .project__certs h3 {
    font-size: 1rem;
    margin-bottom: 1rem;
    color: var(--color-primary-light);
  }

  @media (max-width: 768px) {
    .project__grid {
      grid-template-columns: 1fr;
    }
  }
</style>
