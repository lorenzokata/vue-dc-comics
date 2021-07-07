<template>
  <header>
    <div class="container">

      <img src="../assets/dc-logo.png" alt="logo dc">

      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index" :class="{ active: link.current }"><a href="#">{{link.text}}</a></li>
        </ul>
      </nav>

    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      links: [
        {
          text: 'Characters',
          url: '#',
          current: false
        },
        {
          text: 'Comics',
          url: '#',
          current: false
        },
        {
          text: 'Movies',
          url: '#',
          current: true
        },
        {
          text: 'Tv',
          url: '#',
          current: false
        },
        {
          text: 'Games',
          url: '#',
          current: false
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false
        },
        {
          text: 'Videos',
          url: '#',
          current: false
        },
        {
          text: 'Fans',
          url: '#',
          current: false
        },
        {
          text: 'News',
          url: '#',
          current: false
        },
        {
          text: 'Shop',
          url: '#',
          current: false
        }
      ]
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '@/style/commons.scss';

.container{
  display: flex;
  justify-content: space-between;
  padding: 20px 0;
  
  nav{

    display: flex;
    align-items: center;
    width: 70%;

    ul{

      display: flex;
      align-items: center;
      justify-content: space-around;
      width: 100%;
      height: 100%;

      li{

        list-style: none;
        height: 100%;
        display: flex;
        align-items: center;
        color: black;

        a{

          text-transform: uppercase;
          text-decoration: none;
          font-size: 12px;
          font-weight: bold;
          color: black;
        }

        &.active{
          border-bottom: 5px #0282F9 solid;
        }

        &:hover a,
        &.active a{
          color: #0282F9;
        }
      }
    }
  }
}

</style>