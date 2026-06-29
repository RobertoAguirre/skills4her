<section id="programa" class="section">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">El programa</span>
      <h2>¿Qué es Skills4Her?</h2>
      <p class="section__lead">
        Skills4Her es un programa de formación integral diseñado para mujeres que quieren fortalecer
        sus habilidades tecnológicas, profesionales y personales.
      </p>
    </header>

    <div class="about__grid">
      <div class="about__main">
        <p>
          A lo largo del programa aprenderás sobre software, tecnología, metodologías ágiles,
          habilidades blandas, finanzas personales y empoderamiento femenino en el trabajo.
        </p>
        <p>
          En formato <strong>bootcamp</strong>, desarrollarás herramientas y productos digitales
          aplicando <strong>vibecoding</strong> — un enfoque creativo que te permite construir
          soluciones reales de forma intuitiva, utilizando IA, sin necesidad de experiencia previa en programación.
        </p>
        <p class="about__note">
          No necesitas experiencia previa en programación ni un nivel escolar mínimo. El programa
          está diseñado para acompañarte paso a paso, siempre que tengas compromiso, disponibilidad
          y ganas de aprender.
        </p>
      </div>

      <aside class="about__aside">
        <div class="about__card">
          <div class="about__card-icon" aria-hidden="true">🚀</div>
          <h3>Formato bootcamp</h3>
          <p>18 semanas de formación intensiva con proyectos prácticos y acompañamiento continuo.</p>
        </div>
        <div class="about__card">
          <div class="about__card-icon" aria-hidden="true">✦</div>
          <h3>Vibecoding</h3>
          <p>Crea herramientas y productos digitales con un enfoque creativo, visual e intuitivo.</p>
        </div>
      </aside>
    </div>
  </div>
</section>

<style>
  .about__grid {
    display: grid;
    grid-template-columns: 1fr 320px;
    gap: 2.5rem;
    align-items: start;
  }

  .about__main {
    display: flex;
    flex-direction: column;
    gap: 1.25rem;
    font-size: 1.05rem;
    color: var(--color-text-muted);
    line-height: 1.75;
  }

  .about__main strong {
    color: var(--color-text);
  }

  .about__note {
    padding: 1.25rem 1.5rem;
    background: var(--color-accent-soft);
    border-radius: var(--radius);
    border-left: 4px solid var(--color-accent);
    color: var(--color-text);
    font-size: 0.975rem;
  }

  .about__aside {
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }

  .about__card {
    background: var(--color-surface);
    border: 1px solid var(--color-border);
    border-radius: var(--radius-lg);
    padding: 1.5rem;
    box-shadow: var(--shadow);
  }

  .about__card-icon {
    font-size: 1.5rem;
    margin-bottom: 0.75rem;
  }

  .about__card h3 {
    font-size: 1rem;
    margin-bottom: 0.5rem;
  }

  .about__card p {
    font-size: 0.9rem;
    color: var(--color-text-muted);
    line-height: 1.6;
  }

  @media (max-width: 768px) {
    .about__grid {
      grid-template-columns: 1fr;
    }
  }
</style>
