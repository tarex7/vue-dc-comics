<template>
  <footer>
    <div class="container">
      <div class="row">
        <img id="logo" src="../assets/img/dc-logo-bg.png" alt="dc-logo" />
        <div class="col">
          <h3>DC Comics</h3>
          <ul>
            <li v-for="link in DCComicslinks" :key="link.text">
              <a :href="link.url" :class="{ active: link.current }">
                {{ link.text }}</a
              >
            </li>
          </ul>
          <h3>Shop</h3>
          <ul>
            <li v-for="link in shop" :key="link.text">
              <a href="#">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <h3>DC</h3>
          <ul>
            <li v-for="link in DCLinks" :key="link.text">
              <a :href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <h3>Sites</h3>
          <ul>
            <li v-for="link in sites" :key="link.text">
              <a :href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "TopFooter",
  data() {
    return {
      DCComicslinks: [
        {
          text: "Characters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ],
      DCLinks: [
        {
          text: "Terms of use",
          url: "#",
        },
        {
          text: "Privacy policy(New)",
          url: "#",
          current: true,
        },
        {
          text: "Ad choices",
          url: "#",
        },
        {
          text: "Advertising",
          url: "#",
        },
        {
          text: "Jobs",
          url: "#",
        },
        {
          text: "Subscriptions",
          url: "#",
        },
        {
          text: "Talent Workshops",
          url: "#",
        },
        {
          text: "CPSC Certificates",
          url: "#",
        },
        {
          text: "Ratings",
          url: "#",
        },
        {
          text: "Shop Help",
          url: "#",
        },
        {
          text: "Contact Us",
          url: "#",
        },
      ],
      sites: [
        {
          text: "DC",
          url: "#",
        },
        {
          text: "MAD MAgazine",
          url: "#",
          current: true,
        },
        {
          text: "DC Kids",
          url: "#",
        },
        {
          text: "DC Universe",
          url: "#",
        },
        {
          text: "DC Power Visa",
          url: "#",
        },
      ],
      shop: [{ text: "Shop DC" }, { text: "Shop DC Collectibles" }],
    };
  },
};
</script>

<style lang="scss" scoped>
footer {
  background-image: url(../assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  overflow: hidden;
  position: relative;
  padding: 40px;
  .row {
    display: flex;
    .col {
      margin: 0 20px;
    }

    a:hover {
      color: #fff;
    }
  }
  h3 {
    text-transform: uppercase;
  }
  #logo {
    position: absolute;
    top: -11%;
    left: 53%;
    width: 650px;
  }

  ul {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    margin: 10px 0;
    li a {
      color: gray;
      justify-self: start;
      margin: 5px 0;
    }
  }
}
</style>
