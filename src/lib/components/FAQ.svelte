<script>
  import { faqs } from '../data/content.js';

  let openIndex = $state(null);

  function toggle(index) {
    openIndex = openIndex === index ? null : index;
  }
</script>

<section id="faq" class="section section--alt">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Dudas</span>
      <h2>Preguntas frecuentes</h2>
    </header>

    <div class="faq__list">
      {#each faqs as faq, i}
        <div class="faq__item" class:faq__item--open={openIndex === i}>
          <button
            class="faq__question"
            onclick={() => toggle(i)}
            aria-expanded={openIndex === i}
          >
            <span>{faq.question}</span>
            <span class="faq__icon" aria-hidden="true">{openIndex === i ? '−' : '+'}</span>
          </button>
          {#if openIndex === i}
            <div class="faq__answer">
              <p>{faq.answer}</p>
            </div>
          {/if}
        </div>
      {/each}
    </div>
  </div>
</section>

<style>
  .faq__list {
    max-width: 720px;
    display: flex;
    flex-direction: column;
    gap: 0.75rem;
  }

  .faq__item {
    background: var(--color-surface);
    border: 1px solid var(--color-border);
    border-radius: var(--radius);
    overflow: hidden;
    transition: box-shadow 0.2s;
  }

  .faq__item--open {
    box-shadow: var(--shadow);
    border-color: var(--color-primary-light);
  }

  .faq__question {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 1rem;
    padding: 1.25rem 1.5rem;
    background: none;
    border: none;
    cursor: pointer;
    font-family: var(--font-body);
    font-size: 1rem;
    font-weight: 600;
    color: var(--color-text);
    text-align: left;
    transition: color 0.2s;
  }

  .faq__question:hover {
    color: var(--color-primary);
  }

  .faq__icon {
    flex-shrink: 0;
    width: 1.75rem;
    height: 1.75rem;
    display: flex;
    align-items: center;
    justify-content: center;
    background: var(--color-accent-soft);
    color: var(--color-accent);
    border-radius: 50%;
    font-size: 1.1rem;
    font-weight: 700;
  }

  .faq__answer {
    padding: 0 1.5rem 1.25rem;
  }

  .faq__answer p {
    font-size: 0.95rem;
    color: var(--color-text-muted);
    line-height: 1.65;
  }
</style>
