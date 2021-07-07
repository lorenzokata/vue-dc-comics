<template>

  <div class="book-card">
    <img :src="book.thumb" :alt="book.series + ' ' + book.type">
    <span>{{ book.series}}</span>
  </div>

</template>


<script>

export default {
  name: 'BookCard',
  props: ['book'],
}

</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '@/style/commons.scss';

.book-card{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 10px;

  span{
    align-self: flex-start;
    padding-top: 10px;
    max-width: 192px;
  }
}

</style>