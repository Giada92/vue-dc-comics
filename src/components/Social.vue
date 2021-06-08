<template>
  <section>
      <div class="container social">
          <div class="sing">
              <span class="button">Sign-Up Now!</span>
          </div>
          <div class="follow">
              <span class="blue">Follow US</span>
              <img src="../assets/img/footer-facebook.png" alt="Icona Facebook">
              <img src="../assets/img/footer-twitter.png" alt="Icona Twitter">
              <img src="../assets/img/footer-youtube.png" alt="Icona YouTube">
              <img src="../assets/img/footer-pinterest.png" alt="Icona Pinterest">
              <img src="../assets/img/footer-periscope.png" alt="Icona Periscope">
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name: "Social"
}
</script>

<style lang="scss" scoped>
//importo il nome del file dove ho salvato la variabile con lo stile
@import "../style/variabile.scss";
@import "../style/mixins.scss";

section{
    width: 100%;
    height: 100px;
    background-color: #303030;
}

.social {
    display: flex;
    height: 100%;
}

.sing,
.follow {
    display: flex;
    align-items: center;
    width: 50%;
    height: 100%;
}

.follow {
    justify-content: flex-end
}

img {
    padding: 0 10px;
    cursor: pointer;
    transition: all 1s;
    &:hover{
        opacity: 0.5;
    }
}

span {
    font-weight: 600;
    text-transform: uppercase;
}

.blue {
    color: $mainColor;
}

.button {
    padding: 12px;
    @include my_button;
}

</style>