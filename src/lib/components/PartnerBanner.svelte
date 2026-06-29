<section class="partners" aria-label="Aliados institucionales">
  <div class="partners__inner">
    <img
      src="/S4H_Banner.png"
      alt="Aliados: FICOSEC, Gobierno del Estado de Chihuahua, Democratizamos la Innovación, Desarrollo Económico y Startup Juárez"
      width="1400"
      height="120"
      loading="eager"
    />
  </div>
</section>

<style>
  .partners {
    background: #000;
    padding: 1.25rem 0;
  }

  .partners__inner {
    width: min(100% - 2rem, 1200px);
    margin-inline: auto;
  }

  .partners img {
    width: 100%;
    object-fit: contain;
    max-height: 90px;
  }

  @media (max-width: 640px) {
    .partners {
      overflow-x: auto;
      -webkit-overflow-scrolling: touch;
    }

    .partners__inner {
      width: max-content;
      min-width: 100%;
      padding-inline: 1rem;
    }

    .partners img {
      min-width: 700px;
      max-height: 70px;
    }
  }
</style>
