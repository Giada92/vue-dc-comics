<template>
  <header>
      <div class="container cols">
        <div id="logo">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>
        <nav>
            <ul>
                <li v-for="(link, index) in links"  :key="index"
                @click="changeNavStatus(index)" :class="{active: index==activeIndex}">
                    <a :href="link.url" :class="{active: index==activeIndex}">{{ link.name }}</a>
                </li>
            </ul>
        </nav>
      </div>
    </header>
</template>

<script>
export default {
    name: 'MenuLogo',
    props: {
        links: Array
    },
    data: function() {
        return {
            activeIndex: 0,
        }
    },
    methods: {
        changeNavStatus: function(index){
            return (this.activeIndex = index);
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variabile.scss";

header {
    height: 100px;
}

.cols {
    height: 100%;
    display: flex;
    justify-content: space-between;
    line-height: 94px;
}

#logo{
    width: 30%;
    height: 100%;
    cursor: pointer;

    img {
        height: 80%;
        vertical-align: middle;
    }
}

ul {
    display: flex;

    li {
        list-style: none;
        margin: 0 10px;
        &:hover,
        &.active {
            border-bottom: 5px solid $mainColor;
        }

        a {
            text-decoration: none;
            text-transform: uppercase;
            font-size: 13px;
            font-weight: 600;
            color: #555051;
            &:hover,
            &.active {
                color: $mainColor;
            }
        }
    }
}

</style>