<template>
  <main>
    <HeaderComponent />
    <section class="d-flex flex-column justify-content-center align-items-center mt-5">
      <h2>Serviços em até 4 horas!</h2>
      <article class="d-flex w-50">
        <CarrosselSlider class="my-5" />
      </article>
    </section>
  </main>
</template>

<script>
export default {
  components: {
    HeaderComponent: () => import("../components/HeaderComponent.vue"),
    CarrosselSlider: () => import("../components/CarrosselSlider.vue"),
  }
}
</script>

<style>

</style>