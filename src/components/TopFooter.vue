<template>
  <footer>
    <div class="container">
      <div class="row">
        <img id="logo" src="../assets/img/dc-logo-bg.png" alt="dc-logo" />
        <div class="col">
          <h3>DC Comics</h3>
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
          <h3>Shop</h3>
          <ul>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop Dc Collectibles</a></li>
          </ul>
        </div>
        <div class="col">
          <h3>DC Comics</h3>
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
        <div class="col">
          <h3>Sites</h3>
          <ul>
            <li><a href="#">Characthers</a></li>
            <li><a class="active" href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "TopFooter",
};
</script>

<style lang="scss" scoped>
footer {
  background-image: url(../assets/img/footer-bg.jpg);
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
    margin: 15px 0;
  }
  #logo {
    position: absolute;
    top: -10%;
    left: 53%;
    width: 27%;
  }

  ul {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    li a {
      color: gray;
      justify-self: start;
    }
  }
}
</style>
