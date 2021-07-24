<template>
    <div class="container__credits">
      <section class="credits__flaticon">
        Iconos diseñados por
        <a
          href="https://www.flaticon.es/autores/pixel-perfect"
          title="Pixel perfect"
          target="_blank"
        >
          Pixel perfect
        </a>
        from
        <a href="https://www.flaticon.es/" title="Flaticon" target="_blank"
          >www.flaticon.es</a
        >
      </section>
      <section class="credits__user">sitio diseñado por jochizan</section>
    </div>
</template>

<style>
    .list__details {
  list-style: none;
  display: grid;
  grid-template: auto / repeat(auto-fit, minmax(48px, 160px));
  align-content: center;
  justify-content: center;
  gap: 8rem;
}

.list__details li {
  background: var(--border-color);
  border-radius: 20px;
  box-shadow: rgba(17, 17, 26, 0.1) 0px 4px 16px, rgba(17, 17, 26, 0.1) 0px 8px 24px, rgba(17, 17, 26, 0.1) 0px 16px 56px;
}

.list__details li p {
  text-align: center;
  color: var(--text-color);
  font-size: 1.4rem;
}

.container__credits {
  padding: 1rem;
  border: none;
  border-radius: 0;
  background: transparent;
  color: var(--text-color);
  display: grid;
  font-size: 1.2rem;
  grid-template: auto / repeat(2, 1fr);
  justify-content: center;
  align-content: center;
}

.container__credits section {
  align-self: center;
  display: flex;
  justify-content: center;
}

</style>