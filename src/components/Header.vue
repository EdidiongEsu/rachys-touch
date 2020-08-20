<template>
  <div id="nav">
    <b-navbar toggleable="lg" type="dark" class="nav-background">
      <b-navbar-brand
        id="brand-name"
        href="#"
        tag="h1"
        class="mx-auto text-center center-block navbar-brand"
      >
        <img src="../assets/images/logo.png" class="d-inline-block align-top" />
        RACHY'S TOUCH
      </b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="#" class="mr-2">HOME</b-nav-item>
          <b-nav-item href="#" class="mr-2">ABOUT</b-nav-item>
          <b-nav-item href="#">CONTACT</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {},
};
</script>

<style>
.nav-background {
  background: rgb(41, 39, 39);
  font-family: "Playfair Display", serif;
}
b-navbar-nav {
  background-color: white !important;
}
b-navbar-brand {
  font-size: 100px !important;
}
img {
  height: 40px;
}

@media (min-width: 992px) {
  .navbar-brand {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
  }
}
</style>
