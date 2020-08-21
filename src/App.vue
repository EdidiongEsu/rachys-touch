<template>
  <div id="app">
    <!--Homepage-->
    <header>
      <div>
        <top-header />
        <Carousel />
      </div>
    </header>
  </div>
</template>

<script>
import Header from "./components/Header";
import Carousel from "./components/Carousel";
export default {
  name: "App",
  components: {
    "top-header": Header,
    Carousel,
  },
  methods: {},
};
</script>

<style lang="scss">
@import "@/scss/main.scss";
header {
  height: 100vh;
}
</style>
