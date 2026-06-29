<script>
  import { learningAreas } from '../data/content.js';
</script>

<section id="aprendizaje" class="section section--alt">
  <div class="container">
    <header class="section__header">
      <span class="section__eyebrow">Currículo</span>
      <h2>¿Qué aprenderás?</h2>
      <p class="section__lead">
        Cinco áreas de formación que te preparan para construir, liderar y crecer en el mundo
        digital.
      </p>
    </header>

    <div class="card-grid">
      {#each learningAreas as area}
        <article class="card">
          <div class="card__icon" aria-hidden="true">{area.icon}</div>
          <h3>{area.title}</h3>
          <p>{area.description}</p>
        </article>
      {/each}
    </div>
  </div>
</section>
