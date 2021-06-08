<template>
    <div class="bg">
        <div class="container wrapp_footer">
            <div class="links">
                <div class="link">
                    <h4>Dc Comics</h4>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <h4>Shop</h4>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>
                    </ul>
                </div>
                <div class="link">
                    <h4>Dc</h4>
                    <ul>
                        <li>Terms of Use</li>
                        <li>privacy policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Hepl</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="link">
                    <h4>Sites</h4>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
            <div class="logo_footer"></div>
        </div>
    </div>
</template>

<script>
export default {
    name: "Footer"
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
    color: white;
}

ul {
    list-style: none;
    li {
        padding: 2px;
        font-size: 12px;
        color: #6B6160;
        cursor: pointer;
        
        &:hover {
            color: $mainColor;
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