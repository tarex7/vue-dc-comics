<template>
  <div class="banner">
    <div class="container">
      <div class="banner-icons">
        <div v-for="(item, index) in bannerItems" :key="index" class="media">
          <a href="#">
            <img :src="item.src" :alt="item.text" />
            <p class="media-text">{{ item.text }}</p>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BaseBanner",
  data() {
    return {
      bannerItems: [
        {
          src: require("../assets/img/buy-comics-digital-comics.png"),
          text: "Digital comics",
          url: "#",
        },
        {
          src: require("../assets/img/buy-comics-merchandise.png"),
          text: "Dc merchandise",
          url: "#",
        },
        {
          src: require("../assets/img/buy-comics-subscriptions.png"),
          text: "Subscription",
          url: "#",
        },
        {
          src: require("../assets/img/buy-comics-shop-locator.png"),
          text: "Comic shop locator",
          url: "#",
        },
        {
          src: require("../assets/img/buy-dc-power-visa.svg"),
          text: "DC power visa",
          url: "#",
        },
      ],
    };
  },
  computed: {
    image() {
      return require(`../assets/img/${this.items.src}.png`);
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/vars";
.banner {
  background-color: $primary-color;
  padding: 40px;

  .banner-icons {
    display: flex;
    justify-content: space-evenly;
  }

  img {
    width: 60px;
    height: 60px;
    object-fit: contain;
  }

  .media-text {
    text-transform: uppercase;
    margin-left: 5px;
  }

  a {
    color: #fff;
    display: flex;
    align-items: center;
    transition: all 0.2s;

    &:hover {
      transform: scale(1.1);
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
