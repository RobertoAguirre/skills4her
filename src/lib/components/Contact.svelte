<script>
  import PartnerBanner from './PartnerBanner.svelte';
</script>

<section id="contacto" class="section">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Soporte</span>
      <h2>Contacto</h2>
      <p class="section__lead">Para dudas o mayor información:</p>
    </header>

    <div class="contact__card">
      <div class="contact__person">
        <h3>Brenda Holguín</h3>
        <p class="contact__role">Coordinadora de programa</p>
      </div>
      <div class="contact__details">
        <a href="mailto:bholguin@changeandcode.com" class="contact__link">
          <span class="contact__label">Correo</span>
          bholguin@changeandcode.com
        </a>
        <a href="https://wa.me/526144650998" class="contact__link" target="_blank" rel="noopener noreferrer">
          <span class="contact__label">WhatsApp</span>
          614 465 0998
        </a>
      </div>
    </div>
  </div>
</section>

<footer class="footer">
  <div class="container footer__inner">
    <p class="footer__credits">
      Skills4Her es un programa de <strong>Democratizamos la Innovación A.C.</strong>, con
      financiamiento de <strong>FICOSEC Zona Norte</strong> y la
      <strong>Secretaría de Innovación y Desarrollo Económico</strong> a través de la
      <strong>Dirección de Emprendimiento y Desarrollo Empresarial</strong>.
    </p>
    <p class="footer__allies">
      Aliados institucionales: Frente Norte, Startup Juárez, Red Juárez Emprende, Change and Code.
    </p>
    <p class="footer__copy">© 2026 Skills4Her · Ciudad Juárez, Chihuahua</p>
  </div>
  <PartnerBanner lazy />
</footer>

<style>
  .contact__card {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    align-items: center;
    justify-content: space-between;
    background: var(--color-surface);
    border: 1px solid var(--color-border);
    border-radius: var(--radius-lg);
    padding: 2rem;
    box-shadow: var(--shadow);
    max-width: 720px;
  }

  .contact__person h3 {
    font-size: 1.25rem;
    margin-bottom: 0.25rem;
  }

  .contact__role {
    font-size: 0.9rem;
    color: var(--color-text-muted);
  }

  .contact__details {
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
  }

  .contact__link {
    display: flex;
    flex-direction: column;
    text-decoration: none;
    color: var(--color-primary);
    font-weight: 600;
    transition: color 0.2s;
  }

  .contact__link:hover {
    color: var(--color-accent);
    text-decoration: none;
  }

  .contact__label {
    font-size: 0.75rem;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: 0.06em;
    color: var(--color-text-muted);
    margin-bottom: 0.15rem;
  }

  .footer {
    background: var(--color-dark);
    color: #a89bc0;
    padding-block: 2.5rem 0;
    font-size: 0.875rem;
    line-height: 1.7;
  }

  .footer__inner {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    text-align: center;
    padding-bottom: 2.5rem;
  }

  .footer__credits strong,
  .footer__allies {
    color: #d4c8e8;
  }

  .footer__copy {
    margin-top: 0.5rem;
    font-size: 0.8rem;
    opacity: 0.6;
  }
</style>
