<template>
  <div id="nav" class="navigation-bar">
    <b-navbar toggleable="lg" type="dark" class="nav-background">
      <div>
        <b-nav align="left">
          <b-nav-item href="https://www.instagram.com/ellacute22/">
            <i class="fab fa-instagram p-0"></i>
          </b-nav-item>
          <b-nav-item href="https://web.facebook.com/groups/555683488249245">
            <i class="fab fa-facebook p-0"></i>
          </b-nav-item>
        </b-nav>
      </div>
      <b-navbar-brand
        id="brand-name"
        href="#"
        tag="h1"
        class="mx-auto text-center center-block navbar-brand"
      >
        <img src="../assets/images/logo.png" class="d-inline-block align-top logo-img" />
        RACHY'S TOUCH
      </b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="#homepage" class="mr-2 quick-links">HOME</b-nav-item>
          <b-nav-item href="#about" class="mr-2">ABOUT</b-nav-item>
          <b-nav-item href="#contact">CONTACT</b-nav-item>
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
.navigation-bar {
  height: 20%;
}
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
.logo-img {
  height: 40px;
}
.nav-link {
  padding: 0.5rem 0.5rem !important;
}
.navbar-toggler-icon {
  width: 1em;
  height: 1em;
}
.fa-facebook {
  color: red;
}
.fa-instagram {
  color: red;
}

.fa-facebook:hover,
.fa-instagram:hover {
  color: whitesmoke;
}

@media (min-width: 992px) {
  .navbar-brand {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
  }
  .nav-link {
    padding: 1rem 1rem !important;
  }
}
</style>
