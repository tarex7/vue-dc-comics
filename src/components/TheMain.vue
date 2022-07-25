<template>
  <main>
    <div class="container">
      <div class="comics">
        <div class="card" v-for="(comic, i) in comics" :key="i">
          <figure>
            <a href="#"> <img :src="comic.thumb" :alt="comic.series" /></a>
          </figure>
          <figcaption>{{ comic.series }}</figcaption>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "TheMain",
  props: {
    comics: Object,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/vars";

main {
  background-color: #1c1c1c;
  padding: 70px;
  color: #fff;

  .comics {
    .card {
      width: calc(100% / 6);
      margin-bottom: 50px;
      &:hover {
        color: $primary-color;
      }

      &:hover figure {
        border: 3px solid $primary-color;
      }
    }
    display: flex;
    flex-wrap: wrap;
    figure {
      max-height: 186px;
      max-width: 186px;
      overflow: hidden;
      margin: 0px;
      border: 3px solid transparent;
    }
    figcaption {
      text-transform: uppercase;
      margin-top: 20px;
      width: 90%;
    }
  }
}
</style>
