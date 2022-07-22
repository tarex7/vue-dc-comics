<template>
  <div class="banner">
    <div class="container">
      <div class="banner-icons">
        <div class="media">
          <img
            src="../assets/img/buy-comics-digital-comics.png"
            alt="buy-comics-digital-comics"
          />
          <p class="media-text">Digital comics</p>
        </div>
        <div class="media">
          <img
            src="../assets/img/buy-comics-merchandise.png"
            alt="buy-comics-merchandise"
          />
          <p class="media-text">Dc merchandise</p>
        </div>

        <div class="media">
          <img
            src="../assets/img/buy-comics-subscriptions.png"
            alt="buy-comics-subscriptions"
          />
          <p class="media-text">Subscription</p>
        </div>

        <div class="media">
          <img
            src="../assets/img/buy-comics-shop-locator.png"
            alt="buy-comics-shop-locator"
          />
          <p class="media-text">Comic shop locator</p>
        </div>

        <div class="media">
          <img
            id="dc-power"
            src="../assets/img/buy-dc-power-visa.svg"
            alt="buy-dc-power-visa"
          />
          <p class="media-text">Dc power visa</p>
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
    justify-content: space-between;
  }

  img {
    width: 60px;
    height: 60px;
    object-fit: contain;
  }

  .media-text {
    text-transform: uppercase;
    font-size: 0.8rem;
    margin-left: 0px;
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
