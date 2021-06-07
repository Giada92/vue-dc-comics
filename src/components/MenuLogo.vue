<template>
  <header>
      <div id="container" class="cols">
        <div id="logo">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>
        <nav>
            <ul>
                <li v-for="(link, index) in links" :key="index">
                    <a :href="link.url" :class="{active: link.current}">{{ link.name }}</a>
                </li>
            </ul>
        </nav>
      </div>
    </header>
</template>

<script>
export default {
    name: 'MenuLogo',
    data: function() {
        return {
            links: [
                {
                    name: "Characters",
                    url: "#Characters",
                    current: true
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
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
header {
    height: 100px;
    background-color: palegreen;
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
        &:hover {
            border-bottom: 5px solid #0282F9;
        }

        a {
            text-decoration: none;
            text-transform: uppercase;
            font-size: 13px;
            font-weight: 600;
            color: #555051;
            &:hover,
            &.active {
                color: #0282F9;
            }
        }
    }
}

</style>