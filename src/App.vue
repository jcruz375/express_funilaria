<template>
  <div id="app">
    <HomePage />
    <DiferenciaisPage />
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
    HomePage: () => import('./pages/HomePage'),
    DiferenciaisPage: () => import('./pages/DiferenciaisPage.vue'),
  }
};
</script>

<style lang="scss" scoped>
// @import './sass/global.scss';
  #app {
    overflow-x: hidden;
  }
</style>
