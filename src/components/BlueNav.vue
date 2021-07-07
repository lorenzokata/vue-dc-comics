<template>
  <section>
    <div class="container">
      <ul>
        <li v-for="(image,index) in source" :key="index">
          <img :src="source.src" :alt="source.description">
          <span>{{ source.description }}</span>
        </li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: 'BlueNav',
  data() {
    return {
      source:[
        {
          src:'../src/assets/buy-comics-digital-comics.png',
          description: 'Digital Comics'
        },
        {
          src:'../assets/buy-comics-merchandise.png',
          description: 'DC Merchandise'
        },
        {
          src:'../assets/buy-comics-subscription.png',
          description: 'Subscription'
        },
        {
          src:'../assets/buy-comics-shop-locator.png',
          description: 'Comic Shop Locator'
        },
        {
          src:'../assets/buy-dc-power-visa.png',
          description: 'DC Power Visa'
        }
      ]
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
  }

}

</style>