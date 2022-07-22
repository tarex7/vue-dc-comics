<template>
  <div class="banner">
    <div class="container">
      <div class="banner-icons">
        <div class="media">
          <img
            src="../assets/img/buy-comics-digital-comics.png"
            alt="buy-comics-digital-comics"
          />
          <p class="media-text"><a href="#">Digital comics</a></p>
        </div>
        <div class="media">
          <img
            src="../assets/img/buy-comics-merchandise.png"
            alt="buy-comics-merchandise"
          />
          <p class="media-text"><a href="#">Dc merchandise</a></p>
        </div>

        <div class="media">
          <img
            src="../assets/img/buy-comics-subscriptions.png"
            alt="buy-comics-subscriptions"
          />
          <p class="media-text"><a href="#">Subscription</a></p>
        </div>

        <div class="media">
          <img
            src="../assets/img/buy-comics-shop-locator.png"
            alt="buy-comics-shop-locator"
          />
          <p class="media-text"><a href="#">Comic shop locator</a></p>
        </div>

        <div class="media">
          <img
            id="dc-power"
            src="../assets/img/buy-dc-power-visa.svg"
            alt="buy-dc-power-visa"
          />
          <p class="media-text"><a href="#">Dc power visa</a></p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BaseBanner",
};
</script>

<style lang="scss" scoped>
.banner {
  background-color: #0282f9;
  padding: 60px;

  .banner-icons {
    display: flex;
    justify-content: space-evenly;
  }

  img {
    width: 80px;
    height: 80px;
    object-fit: contain;
  }

  .media-text {
    text-transform: uppercase;
    margin-left: 0px;
  }

  a {
    color: #fff;
    &:hover {
      color: #000;
    }
  }

  #dc-power {
    width: 30%;
    margin-right: 5px;
  }

  .media {
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 15px;
  }
}
</style>
