<template>
        <div class="card">
            <img :src="fumetti.thumb" alt="fumetti.series">
            <div class="series">
                <p>{{fumetti.series}}</p>
            </div>
        </div>
</template>

<script>
export default {
    name: "Card",
    props: {
        fumetti: Object
    }
}
</script>

<style lang="scss" scoped>
.card{
    width: calc(100% / 6 - 20px);
    margin: 10px;
    height: 180px;
    overflow: hidden;
    background-color: blue;

    img {
        width: 100%;
        height: 100%;
        display: block;
        object-fit: cover;
        object-position: top;
    }
}


</style>