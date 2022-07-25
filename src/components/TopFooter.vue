<template>
  <footer>
    <div class="container">
      <div class="row">
        <img id="logo" src="../assets/img/dc-logo-bg.png" alt="dc-logo" />
        <div class="col">
          <h3>DC Comics</h3>
          <ul>
            <li v-for="link in DCComicsLinks" :key="link.text">
              <a :href="link.url" :class="{ active: link.current }">
                {{ link.text }}</a
              >
            </li>
          </ul>
          <h3>Shop</h3>
          <ul>
            <li v-for="link in shopLinks" :key="link.text">
              <a href="#">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <h3>DC</h3>
          <ul>
            <li v-for="link in DClinks" :key="link.text">
              <a :href="link.url">{{ link.text }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <h3>Sites</h3>
          <ul>
            <li v-for="link in sitesLinks" :key="link.text">
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

  props: {
    DCComicsLinks: Array,
    DClinks: Array,
    sitesLinks: Array,
    shopLinks: Array,
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
