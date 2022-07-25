<template>
  <div class="container">
    <header class="">
      <nav>
        <a href="#">
          <img id="logo" src="../assets/img/dc-logo.png" alt="logo"
        /></a>
        <div class="links">
          <ul>
            <li v-for="link in mainMenuLinks" :key="link.text">
              <a :href="link.url" :class="{ active: link.current }">
                {{ link.text }}</a
              >
            </li>
          </ul>
        </div>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "BaseHeader",

  props: {
    mainMenuLinks: Array,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/vars";

.active {
  color: $primary-color;
  border-bottom: 8px solid $primary-color;
}
header {
  height: 120px;
  display: flex;
  padding: 20px 0;

  a:hover {
    color: $primary-color;
  }
}
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  width: 100%;

  #logo {
    width: 90px;
  }

  ul {
    line-height: 70px;
    height: 100%;
  }

  li {
    height: 120px;
    line-height: 120px;
    a {
      color: #000;
      text-transform: uppercase;
      font-weight: bold;
      margin: 0 10px;
      height: 100%;
    }
  }
}
</style>
