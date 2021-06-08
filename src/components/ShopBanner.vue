<template>
  <section>
        <div class="container">
            <div class="shop">
                <div class="wrapper_shop">
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="Icona Pad">
                    <span>Digital Comics</span>
                </div>
                <div class="wrapper_shop">
                    <img src="../assets/img/buy-comics-merchandise.png" alt="Icona maglietta">
                    <span>Dc Merchandise</span>
                </div>
                <div class="wrapper_shop">
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="Icona carte">
                    <span>Subscription</span>
                </div>
                <div class="wrapper_shop">
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="Icona indicatore">
                    <span>Comic shop locator</span>
                </div>
                <div class="wrapper_shop">
                    <img class="last_img" src="../assets/img/buy-dc-power-visa.svg" alt="Icona carta di credito">
                    <span>Dc Power Visa</span>
                </div>
            </div>
        </div>
  </section>
</template>

<script>
export default {
    name: "ShopBanner"
}
</script>

<style lang="scss" scoped>
@import "../style/variabile.scss";

section {
    width: 100%;
    height: 120px;
    background-color: $mainColor;
}

.shop {
    height: 120px;
    display: flex;
    justify-content: space-around;
    align-items: center;

    .wrapper_shop {
        display: flex;
        align-items: center;
        height: 100%;

            img {
                height: 40%;
            }

            span {
                margin-left: 10px;
                font-size: 14px;
                text-transform: uppercase;
                color: $lightColor;
            }

            &:last-child img {
                width: 50px;
            }

            &:hover {
                cursor: pointer;
            }
    }
}

</style>