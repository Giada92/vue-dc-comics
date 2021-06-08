<template>
    <div class="bg">
        <div class="container wrapp_footer">
            <div class="links">
                <div class="link">
                    <h4>Dc Comics</h4>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">ideos</a></li>
                        <li><a href="#">Comics</a></li>
                    </ul>
                    <h4>Shop</h4>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="link">
                    <h4>Dc</h4>
                    <ul>
                        <li><a href="#">Terms of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Hepl</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>
                <div class="link">
                    <h4>Sites</h4>
                    <ul>
                        <li v-for="element, index in esempio" :key="index">
                            <a href="#">{{element.name}}</a>
                        </li>
                    </ul>
                    <!-- <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul> -->
                </div>
            </div>
            <div class="logo_footer"></div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Footer",
    props: {
        esempio: Array
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variabile.scss";
.bg {
    height: 300px;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: contain;
    background-position: 0 -75px;
    background-attachment: fixed;
}

.wrapp_footer {
    height: 300px;
    display: flex;
}

.links {
    display: flex;
    width: 40%;
    height: 100%;
    padding-top: 30px;

    .link {
    margin-right: 20px;
}
}

h4 {
    text-transform: uppercase;
    margin: 10px 0;
    color: $lightColor;
}

ul {
    list-style: none;
    li {
            a{
                font-size: 13px;
                cursor: pointer;
                text-decoration: none;
                color: #6B6160;
                &:hover {
                color: $mainColor;
            }
        }
        
    }
}

.logo_footer {
    width: 60%;
    height: 100%;
    background-image: url('../assets/img/dc-logo-bg.png');
    background-repeat: no-repeat;
    background-position: center;
}

</style>