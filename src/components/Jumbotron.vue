<template>
    <div class="wrapper_bg">
       <!-- <div v-for="(i, index) in [activeIndex]" :key="index">
           <img :src="slides[activeIndex].image" alt="">
            <a class="prev" @click="prev()" href="#">Previous</a>
            <a class="next" @click="next()" href="#">Next</a>
       </div> -->
    </div>
</template>

<script>
export default {
    name: "Jumbotron",
/*     data: function(){
        return{
            slides: [
                {
                    image: require("../assets/img/img_1.jpg"),
                    title: "Primo Titolo",
                    subtitle: "Secondo Titolo"
                },
                {
                    image: require("../assets/img/img_2.jpg"),
                    title: "Primo Titolo",
                    subtitle: "Secondo Titolo"
                },
                {
                    image: require("../assets/img/img_3.jpg"),
                    title: "Primo Titolo",
                    subtitle: "Secondo Titolo"
                },
                {
                    image: require("../assets/img/jumbotron.jpg"),
                    title: "Primo Titolo",
                    subtitle: "Secondo Titolo"
                }
            ],
            activeIndex: 0
        } */
    /* },
    methods: {
        next: function(){
            console.log("clicco qui");
            this.activeIndex++;
        }
    } */
}
</script>

<style lang="scss" scoped>
.wrapper_bg {
    width: 100%;
    height: 400px;
    overflow: hidden;
    position: relative;
    background-image: url("../assets/img/jumbotron.jpg");
    background-color: wheat;
    background-position-x: center;
}

img {
    object-fit: contain;
    object-position: center -50px;
}

/* a{
    position: absolute;
    top: 100px;
} */

</style>