<template>
  <div id="app">
    <!-- Intestazione - Logo - Barra di navigazione -->
    <MenuLogo :links="menu" />
    <!-- /Intestazione - Logo - Barra di navigazione -->

    <!-- Main -->
    <main>
      <Jumbotron />
      <WorldDc />
    </main>
    <!-- /Main -->

    <!-- Shop -->
    <ShopBanner />
    <!-- /Shop -->

    <!-- Footer -->
    <footer>
      <!-- Footer Top -->
      <FooterTop :esempio="menu"/>
      <!-- /Footer Top -->

      <!-- Barra social -->
      <Social />
      <!-- /Barra social -->
    </footer>
    <!-- Footer -->

  </div>
</template>

<script>
import MenuLogo from './components/MenuLogo.vue';
import Jumbotron from './components/Jumbotron.vue';
import WorldDc from './components/WorldDc.vue';
import ShopBanner from './components/ShopBanner.vue';
import FooterTop from './components/FooterTop.vue';
import Social from './components/Social.vue';


export default {
  name: 'App',
  components: {
    MenuLogo,
    WorldDc,
    ShopBanner,
    FooterTop,
    Social,
    Jumbotron
  },
  data: function(){
    return {
     menu: [
            {
                name: "Characters",
                url: "#Characters",
                current: false
            },
            {
                name: "Comics",
                url: "#Comics",
                current: false
            },
            {
                name: "Movies",
                url: "#Movies",
                current: false
            },
            {
                name: "Tv",
                url: "#Tv",
                current: false
            },
            {
                name: "Games",
                url: "#Games",
                current: false
            },
            {
                name: "Collectibles",
                url: "#Collectibles",
                current: false
            },
            {
                name: "Videos",
                url: "#Videos",
                current: false
            },
            {
                name: "Fans",
                url: "#Fans",
                current: false
            },
            {
                name: "News",
                url: "#News",
                current: false
            },
            {
                name: "Shop",
                url: "#Shop",
                current: false
            }
        ],
    }
  }
}
</script>

<style lang="scss">

@import "./style/general.scss";

</style>
