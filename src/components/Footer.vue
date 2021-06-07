<template>
  <footer>
        <div class="bg">
            <div id="container" class="wrapp_footer">
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
  </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style lang="scss" scoped>
footer {
    height: 350px;
    background-image: url('../assets/img/footer-bg.jpg');
}

.wrapp_footer {
    height: 350px;
    display: flex;
}

.links {
    display: flex;
    width: 40%;
    height: 100%;
    margin-top: 40px;
}

.link {
    margin: 0 10px;
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
        color: #6B848C;
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