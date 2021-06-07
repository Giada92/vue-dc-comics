<template>
  <div id="app">
    <!-- Intestazione - Logo - Barra di navigazione -->
    <MenuLogo />
    <!-- /Intestazione - Logo - Barra di navigazione -->

    <!-- Main -->
    <WorldDc />
    <!-- /Main -->

    <!-- Shop -->
    <ShopBanner />
    <!-- /Shop -->

    <!-- Footer -->
    <Footer />
    <!-- Footer -->

    <!-- Barra social -->
    <Social />
    <!-- /Barra social -->

  </div>
</template>

<script>
import MenuLogo from './components/MenuLogo.vue';
import WorldDc from './components/WorldDc.vue';
import ShopBanner from './components/ShopBanner.vue';
import Footer from './components/Footer.vue';
import Social from './components/Social.vue';


export default {
  name: 'App',
  components: {
    MenuLogo,
    WorldDc,
    ShopBanner,
    Footer,
    Social
  }
}
</script>

<style lang="scss">

@import "./style/general.scss";

</style>
