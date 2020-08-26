<template>
  <div id="app">
    <!--Homepage-->
    <header id="homepage">
      <div>
        <top-header />
        <Carousel />
      </div>
    </header>
    <main>
      <about-us id="about" />
      <Gallery id="gallery" />
      <Footer id="footer" />
    </main>
  </div>
</template>

<script>
import Header from "./components/Header";
import Carousel from "./components/Carousel";
import About from "./components/About";
import Gallery from "./components/Gallery";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    "top-header": Header,
    Carousel,
    "about-us": About,
    Gallery,
    Footer,
  },
  methods: {},
};
</script>


<style lang="scss">
@import "@/scss/main.scss";
</style>
