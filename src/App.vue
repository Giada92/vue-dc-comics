<template>
  <div id="app">
    <!-- Intestazione - Logo - Barra di navigazione -->
    <MenuLogo />
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
      <FooterTop />
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
  }
}
</script>

<style lang="scss">

@import "./style/general.scss";

</style>
