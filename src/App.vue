<template>
  <div id="app">
    <HomePage />
    <DiferenciaisPage />
    <ServicosPage />
    <FooterComponent />
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
    HomePage            : () => import('./pages/HomePage'),
    DiferenciaisPage    : () => import('./pages/DiferenciaisPage.vue'),
    ServicosPage        : () => import('./pages/ServicosPage.vue'),
    FooterComponent     : () => import('./components/FooterComponent.vue'),
  }
};
</script>

<style lang="scss" scoped>
// @import './sass/global.scss';
  #app {
    overflow-x: hidden;
  }
</style>
