<template>
  <section>
    <div class="container">
      <div class="contents">Content goes here</div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ItemsGallery',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../../style/commons.scss';

section{
  background-color: black;
  padding: 40px 0;

  .contents{
    color: white;
    font-weight: bold;
  }
}

</style>