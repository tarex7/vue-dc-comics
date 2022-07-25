<template>
  <div>
    <BaseHeader />
    <BaseJumbotron />
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
import BaseJumbotron from "./components/BaseJumbotron.vue";

export default {
  name: "App",
  components: {
    BaseHeader,
    TheMain,
    BaseBanner,
    TopFooter,
    BottomFooter,
    BaseJumbotron,
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
