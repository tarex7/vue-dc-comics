<template>
  <div class="container">
    <header class="">
      <nav>
        <a href="#">
          <img id="logo" src="../assets/img/dc-logo.png" alt="logo"
        /></a>
        <div class="links">
          <ul>
            <li><a href="#">Characthers</a></li>
            <li><a class="active" href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Collectibles</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">Fans</a></li>
            <li><a href="#">News</a></li>
            <li><a href="#">Shop</a></li>
          </ul>
        </div>
      </nav>
    </header>
  </div>
</template>

<script>
export default {
  name: "BaseHeader",
};
</script>

<style lang="scss" scoped>
.active {
  color: #0282f9;
  border-bottom: 8px solid #0282f9;
}
header {
  height: 120px;
  display: flex;
  padding: 20px 0;

  a:hover {
    color: #0282f9;
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
