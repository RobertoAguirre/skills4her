<script>
  import { inPersonDates } from '../data/content.js';
</script>

<section class="section section--alt">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Logística</span>
      <h2>Horarios y modalidad</h2>
      <p class="section__lead">
        El programa se realizará en modalidad híbrida.
      </p>
    </header>

    <div class="schedule__grid">
      <article class="schedule__card">
        <div class="schedule__type">Sesiones virtuales</div>
        <h3>Lunes a jueves</h3>
        <p class="schedule__time">6:00 p.m. – 8:00 p.m.</p>
        <p class="schedule__desc">Clases en línea con acompañamiento continuo durante la semana.</p>
      </article>

      <article class="schedule__card schedule__card--accent">
        <div class="schedule__type">Sesiones presenciales obligatorias</div>
        <h3>Sábados</h3>
        <p class="schedule__time">10:00 a.m. – 1:00 p.m.</p>
        <p class="schedule__desc">En Ciudad Juárez. Fechas presenciales:</p>
        <ul class="schedule__dates">
          {#each inPersonDates as date}
            <li>{date}</li>
          {/each}
        </ul>
        <p class="schedule__note">
          La última sesión presencial será la presentación de los mejores proyectos y entrega de
          constancias.
        </p>
      </article>
    </div>
  </div>
</section>

<style>
  .schedule__grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 1.5rem;
  }

  .schedule__card {
    background: var(--color-surface);
    border: 1px solid var(--color-border);
    border-radius: var(--radius-lg);
    padding: 2rem;
    box-shadow: var(--shadow);
  }

  .schedule__card--accent {
    border-color: var(--color-primary-light);
    background: linear-gradient(135deg, #faf8fc 0%, #f3eeff 100%);
  }

  .schedule__type {
    font-size: 0.75rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.06em;
    color: var(--color-primary);
    margin-bottom: 0.75rem;
  }

  .schedule__card h3 {
    font-size: 1.5rem;
    margin-bottom: 0.5rem;
  }

  .schedule__time {
    font-family: var(--font-display);
    font-size: 1.25rem;
    font-weight: 700;
    color: var(--color-text);
    margin-bottom: 0.75rem;
  }

  .schedule__desc {
    font-size: 0.95rem;
    color: var(--color-text-muted);
    margin-bottom: 1rem;
  }

  .schedule__dates {
    list-style: none;
    display: grid;
    gap: 0.5rem;
    margin-bottom: 1rem;
  }

  .schedule__dates li {
    font-size: 0.9rem;
    padding: 0.5rem 0.75rem;
    background: white;
    border-radius: 8px;
    border: 1px solid var(--color-border);
  }

  .schedule__note {
    font-size: 0.85rem;
    color: var(--color-text-muted);
    font-style: italic;
    border-top: 1px solid var(--color-border);
    padding-top: 1rem;
  }
</style>
