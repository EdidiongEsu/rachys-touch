<template>
  <div id="app">
    <main>
      <Header />
      <Hero />
    </main>
  </div>
</template>

<script>
import Header from "./components/Header";
import Hero from "./components/Hero";
export default {
  name: "App",
  components: {
    Header,
    Hero,
  },
  methods: {
    Celebration: function () {
      alert("This is a cruise!!!");
    },
  },
};
</script>

<style lang="scss">
@import "@/scss/main.scss";
</style>
