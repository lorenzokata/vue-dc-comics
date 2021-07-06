<template>
  <div id="app">
    <Header/>
    <ItemsGallery/>
    <BlueNav/>
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  import ItemsGallery from './components/ItemsGallery.vue'
  import BlueNav from './components/BlueNav.vue'

  export default {
    name: 'App',
    components: {
      Header,
      ItemsGallery,
      BlueNav
    }
  }
</script>

<style lang="scss">

  @import 'style/commons.scss';

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
  }
</style>
