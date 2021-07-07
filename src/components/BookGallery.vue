<template>

  <section id="book-gallery">
    <div class="container">
      <div class="contents">
        <BookCard v-for="(book, index) in books" :key="index" :book="book"/>
      </div>
      <button>Load More</button>
    </div>
  </section>

</template>


<script>

import ComicBooks from '../data/ComicBooks.js';
import BookCard from '../components/BookCard.vue';

export default {
  name: 'BookGallery',
  components: {
    BookCard
  },
  data() {
    return {
      books: ComicBooks
    }
  },
}

</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '@/style/commons.scss';

section{
  background-color: black;
  padding: 40px 0;

  .contents{
    color: white;
    font-weight: bold;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    margin-bottom: 20px;
  }

  button{
    text-align: center;
    padding: 5px 30px;
    background-color: #0282F9;
    color: white;
    text-transform: uppercase;
    border: none;
    font-weight: 900;
  }
}

</style>