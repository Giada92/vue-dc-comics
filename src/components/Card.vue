<template>
    <div class="card">
        <img :src="fumetti.thumb" alt="fumetti.series">
        <p>{{fumetti.series}}</p>
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
@import "../style/variabile.scss";

.card{
    width: calc(100% / 6 - 20px);
    margin: 10px;
    height: 180px;
    margin-top: 20px;
    overflow: hidden;
    cursor: pointer;
    &:hover p{
        color: $mainColor;
    }

    img {
        width: 150px;
        height: 140px;
        display: block;
        object-fit: cover;
        object-position: top;
    }

    p{
        width: 150px;
        padding-top: 10px;
        font-size: 13px;
        text-transform: uppercase;
        color: $lightColor;
    }
}
</style>