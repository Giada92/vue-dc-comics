<template>
  <header>
      <div id="container" class="cols">
        <div id="logo">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>
        <nav>
            <ul>
                <li>
                    <a href="#" class="active">Characters</a>
                </li>
                <li>
                    <a href="#">Comics</a>
                </li>
                <li>
                    <a href="#">Movies</a>
                </li>
                <li>
                    <a href="#">Tv</a>
                </li>
                <li>
                    <a href="#">Games</a>
                </li>
                <li>
                    <a href="#">Collectibles</a>
                </li>
                <li>
                    <a href="#">Videos</a>
                </li>
                <li>
                    <a href="#">Fans</a>
                </li>
                <li>
                    <a href="#">News</a>
                </li>
                <li>
                    <a href="#">Shop</a>
                </li>
            </ul>
        </nav>
      </div>
    </header>
</template>

<script>
export default {
    name: 'MenuLogo'
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
            color: black;
            &:hover,
            &.active {
                color: #0282F9;
            }
        }
    }
}
</style>