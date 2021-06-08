<template>
    <div class="wrapper">
        <div class="container">
            <h2>Current Series</h2>
            <div class="cards">
                <Card 
                v-for="comic, index in comics" :key="index"
                :fumetti="comic"/>
            </div>
            <div class="load">
                <span>Load More</span>
            </div>
        </div>
    </div>
</template>

<script>
import Card from './Card.vue';
import json from '../data/json.js';

export default {
    name: "WorldDc",
    components: {
    Card
  },
  data: function(){
      return {
          comics: json
      }
  }
}
</script>

<style lang="scss" scoped>
@import "../style/variabile.scss";
@import "../style/mixins.scss";

.wrapper {
    width: 100%;
    position: relative;
    display: flex;
    align-items: center;
    background-color: #1C1C1C;
}

h2 {
    position: absolute;
    top: 0;
    transform: translateY(-50%);
    display: inline-block;
    padding: 12px;
    background-color: $mainColor;
    color: $lightColor;
    text-transform: uppercase;
}

.cards {
    width: 100%;
    margin: 30px 0;
    display: flex;
    flex-wrap: wrap;
}

.load{
    width: 100%;
    margin: 20px 0;

    span {
        display: inline-block;
        padding: 12px 40px;
        text-transform: uppercase;
        @include my_button;
}
}
</style>