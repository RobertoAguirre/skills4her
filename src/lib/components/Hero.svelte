<script>
  import { APPLY_URL } from '../data/content.js';
</script>

<section class="hero">
  <div class="hero__bg" aria-hidden="true"></div>
  <div class="container hero__content">
    <div class="hero__badge">Bootcamp · Vibecoding · Ciudad Juárez</div>
    <h1 class="hero__title">
      Aprende tecnología, fortalece tu liderazgo y abre nuevas oportunidades profesionales
    </h1>
    <p class="hero__subtitle">
      <strong>Skills4Her</strong> es un programa de formación para mujeres de Ciudad Juárez que
      desean desarrollar habilidades en tecnología, liderazgo, finanzas personales y empleabilidad
      digital — en un formato bootcamp donde construirás herramientas y productos con
      <em>vibecoding</em>.
    </p>
    <p class="hero__highlight">
      Postúlate para recibir una beca del <strong>100%</strong> y formar parte de una generación de
      mujeres listas para construir soluciones digitales, fortalecer su perfil profesional y avanzar
      en la economía digital.
    </p>

    <div class="hero__meta">
      <div class="hero__meta-item">
        <span class="hero__meta-label">Cupo limitado</span>
        <span class="hero__meta-value">50 beneficiarias</span>
      </div>
      <div class="hero__meta-divider" aria-hidden="true"></div>
      <div class="hero__meta-item">
        <span class="hero__meta-label">Fecha límite</span>
        <span class="hero__meta-value">17 de julio de 2026</span>
      </div>
    </div>

    <div class="hero__actions">
      <a href={APPLY_URL} class="btn btn--primary" target="_blank" rel="noopener noreferrer">
        Quiero postularme
      </a>
      <a href="#programa" class="btn btn--outline">Conocer el programa</a>
    </div>
  </div>
</section>

<style>
  .hero {
    position: relative;
    min-height: 100svh;
    display: flex;
    align-items: center;
    padding-top: var(--header-height);
    padding-bottom: 3rem;
    overflow: hidden;
    background: var(--color-dark);
    color: #f0eaf8;
  }

  .hero__bg {
    position: absolute;
    inset: 0;
    background:
      radial-gradient(ellipse 80% 60% at 20% 40%, rgba(124, 58, 237, 0.35) 0%, transparent 60%),
      radial-gradient(ellipse 60% 50% at 80% 60%, rgba(236, 72, 153, 0.25) 0%, transparent 55%),
      radial-gradient(ellipse 40% 30% at 60% 10%, rgba(20, 184, 166, 0.15) 0%, transparent 50%);
  }

  .hero__content {
    position: relative;
    max-width: 780px;
  }

  .hero__badge {
    display: inline-block;
    padding: 0.4rem 1rem;
    background: rgba(255, 255, 255, 0.08);
    border: 1px solid rgba(255, 255, 255, 0.15);
    border-radius: 999px;
    font-size: 0.8rem;
    font-weight: 600;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    margin-bottom: 1.5rem;
    color: var(--color-primary-light);
  }

  .hero__title {
    font-size: clamp(2rem, 5.5vw, 3.25rem);
    letter-spacing: -0.03em;
    margin-bottom: 1.25rem;
    line-height: 1.15;
  }

  .hero__subtitle {
    font-size: 1.125rem;
    line-height: 1.7;
    color: #c4b8d8;
    margin-bottom: 1rem;
  }

  .hero__subtitle em {
    color: var(--color-teal);
    font-style: normal;
    font-weight: 600;
  }

  .hero__highlight {
    font-size: 1rem;
    color: #a89bc0;
    margin-bottom: 2rem;
    padding-left: 1rem;
    border-left: 3px solid var(--color-accent);
  }

  .hero__meta {
    display: flex;
    align-items: center;
    gap: 1.5rem;
    flex-wrap: wrap;
    margin-bottom: 2.5rem;
    padding: 1.25rem 1.5rem;
    background: rgba(255, 255, 255, 0.05);
    border-radius: var(--radius);
    border: 1px solid rgba(255, 255, 255, 0.1);
  }

  .hero__meta-label {
    display: block;
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 0.06em;
    color: #8b7da8;
    margin-bottom: 0.2rem;
  }

  .hero__meta-value {
    font-family: var(--font-display);
    font-size: 1.1rem;
    font-weight: 700;
    color: white;
  }

  .hero__meta-divider {
    width: 1px;
    height: 2.5rem;
    background: rgba(255, 255, 255, 0.15);
  }

  .hero__actions {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
  }

  @media (max-width: 480px) {
    .hero__meta-divider {
      display: none;
    }
  }
</style>
