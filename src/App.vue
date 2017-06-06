<template>
  <div id="app">
    <app-header></app-header>
    <app-home></app-home>
    <app-footer></app-footer>
  </div>
</template>

<script>
  import Header from './components/header.vue';
  import Home from './components/home.vue';
  import Footer from './components/footer.vue';

  export default {
    components: {
      appHeader: Header,
      appHome: Home,
      appFooter: Footer
    }
  }
</script>

<style lang="scss">
  @import './assets/app.scss';
</style>
