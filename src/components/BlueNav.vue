<template>
  <section>
    <div class="container">
      <ul>
        <li v-for="(image,index) in source" :key="index">
          <img :src="image.src" :alt="image.description">
          <span>{{ image.description }}</span>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>

import BlueNavSource from '../data/BlueNavSource.js'

export default {
  name: 'BlueNav',
  data() {
    return {
      source: BlueNavSource
    }
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '@/style/commons.scss';

section{
  background-color: #0282F9;
  padding: 40px 0;

  ul{
    display: flex;
    justify-content: space-between;
    align-items: center;
    list-style: none;
  }

}

</style>