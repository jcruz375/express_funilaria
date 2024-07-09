<template>
  <div id="app">
    <HomePage />
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
    HomePage: () => import('./pages/HomePage'),
  }
};
</script>

<style lang="scss" scoped>
// @import './sass/global.scss';

</style>
