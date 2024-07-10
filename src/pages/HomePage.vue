<template>
  <main>
    <HeaderComponent />
    <section
      class="d-flex flex-column justify-content-center align-items-center mt-5"
    >
      <h1 class="text-center">Serviços em até 4 horas!</h1>
      <p class="my-1 text-center w-100 w-md-50">
        Utilizando tecnologia de ponta em reparos automotivos, completamos
        serviços de pintura em menos de 4 horas. <br>
        <small>
          *Retoques de pintura rápidos sem necessidade de funilaria ou
          desmontagem.
        </small>
      </p>
      <article class="d-flex w-75 w-md-50">
        <CarrosselSlider class="my-4" />
      </article>
      <a href="https://api.whatsapp.com/send?phone=5511994718878" target="_blank" class="btn-wpp mt-2 mb-5">
        <i class="fab fa-whatsapp"></i>
        saber mais
      </a>
    </section>
  </main>
</template>

<script>
export default {
  components: {
    HeaderComponent: () => import("../components/HeaderComponent.vue"),
    CarrosselSlider: () => import("../components/CarrosselSlider.vue"),
  },
};
</script>

<style lang="scss" scoped>
@import "../sass/global.scss";

  h1 {
    font-size: 2.5rem;
    font-weight: 700;
  }

  p {
    font-size: 1rem;
    padding: 0 1rem;

    small {
      font-size: 0.6rem;
      font-weight: 400;
    }
  }

  @media (max-width: 768px) {
    h1 {
      font-size: 2rem;
    }
  }
</style>