<template>
  <div id="app">
    <!-- Intestazione -->
    <MenuLogo />
    <!-- /Intestazione -->

  </div>
</template>

<script>
import MenuLogo from './components/MenuLogo.vue';


export default {
  name: 'App',
  components: {
    MenuLogo
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
  width: 80%;
  margin: 0 auto;
}

</style>
