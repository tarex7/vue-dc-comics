<template>
  <div>
    <BaseHeader />
    <TheMain />
    <BaseBanner />
    <TopFooter />
    <BottomFooter />
  </div>
</template>

<script>
import BaseHeader from "./components/BaseHeader.vue";
import TheMain from "./components/TheMain.vue";
import BaseBanner from "./components/BaseBanner.vue";
import TopFooter from "./components/TopFooter.vue";
import BottomFooter from "./components/BottomFooter.vue";

export default {
  name: "App",
  components: { BaseHeader, TheMain, BaseBanner, TopFooter, BottomFooter },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.debug {
  border: 1px red solid;
}

body {
  font-family: "Open Sans", sans-serif;
  color: #fff;
}
.container {
  max-width: 1400px;
  margin: 0 auto;
}

img {
  max-width: 100%;
}

ul {
  display: flex;
  list-style-type: none;
  justify-content: center;
  align-items: center;
}

a {
  text-decoration: none;
  display: inline-block;
}
</style>
