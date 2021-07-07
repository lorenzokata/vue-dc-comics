<template>
  <div id="app">
    <Header/>
    <BookGallery/>
    <BlueNav/>
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  import BookGallery from './components/BookGallery.vue'
  import BlueNav from './components/BlueNav.vue'

  export default {
    name: 'App',
    components: {
      Header,
      BookGallery,
      BlueNav
    }
  }
</script>

<style lang="scss">

  @import '@/style/commons.scss';

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
  }
</style>
