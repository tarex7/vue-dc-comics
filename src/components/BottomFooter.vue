<template>
  <footer>
    <div class="container">
      <div class="footer-content">
        <a href="#" class="btn"><h3>Sign-up now</h3></a>
        <div class="social">
          <h3>Follow us</h3>
          <a href="#"
            ><img src="../assets/img/footer-facebook.png" alt="facebook"
          /></a>
          <a href="#"
            ><img src="../assets/img/footer-twitter.png" alt="facebook"
          /></a>
          <a href="#"
            ><img src="../assets/img/footer-youtube.png" alt="facebook"
          /></a>
          <a href="#"
            ><img src="../assets/img/footer-pinterest.png" alt="facebook"
          /></a>

          <a href="#">
            <img src="../assets/img/footer-periscope.png" alt="facebook" />
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  name: "BottomFooter",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/vars";

footer {
  background-color: #303030;
  padding: 50px;
  .footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .social {
      display: flex;
      align-items: center;

      h3 {
        color: $primary-color;
        margin-right: 10px;
      }

      img {
        margin: 0 10px;
        transition: all 0.2s;
        &:hover {
          transform: scale(1.1);
        }
      }
    }
  }
}
h3 {
  text-transform: uppercase;
}

.btn {
  padding: 15px;
  color: #fff;
  border: 3px solid $primary-color;
  transition: all 0.3s;
  &:hover {
    background-color: #fff;
    color: $primary-color;
  }
}
</style>
