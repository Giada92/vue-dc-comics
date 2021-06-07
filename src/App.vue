<template>
  <div id="app">
    <!-- Intestazione - Logo - Barra di navigazione -->
    <MenuLogo />
    <!-- Intestazione - Logo - Barra di navigazione -->

    <!-- Main -->
    <WorldDc />
    <!-- Main -->

    <!-- Footer -->
    <Footer />
    <!-- Footer -->

  </div>
</template>

<script>
import MenuLogo from './components/MenuLogo.vue';
import WorldDc from './components/WorldDc.vue';
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
    MenuLogo,
    WorldDc,
    Footer
  }
}
</script>

<style lang="scss">
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: 'Roboto', sans-serif;
}

#container {
  width: 70%;
  margin: 0 auto;
}

</style>
