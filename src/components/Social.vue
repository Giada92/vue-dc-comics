<template>
  <section>
      <div id="container">
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
section{
    width: 100%;
    height: 100px;
    background-color: #303030;
}

#container {
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
}

span {
    font-weight: 600;
    text-transform: uppercase;
}

.blue {
    color: #0282F9;
}

.button {
    padding: 12px;
    border: 2px solid #0282F9;
    color: white;
}
</style>