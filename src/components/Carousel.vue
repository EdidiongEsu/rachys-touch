<template>
  <div class="carousel">
    <b-carousel id="carousel-fade" style="text-shadow: 0px 0px 2px #000" interval="10000" controls>
      <div class="carousel-inner">
        <b-carousel-slide img-src="../assets/images/img-carousel1.png">
          <div class="brand-carousel">
            <h1 class="display-2">RACHY'S TOUCH COSMETICS</h1>
            <h3 class="mb-1">Beautification, SkinCare and Epidermology</h3>
            <b-button pill class="btn btn-lg mt-1">Gallery</b-button>
            <b-button pill class="btn btn-lg ml-2 mt-1" variant="primary">Contact Us</b-button>
          </div>
        </b-carousel-slide>
        <b-carousel-slide img-src="../assets/images/img-carousel2.png"></b-carousel-slide>
        <b-carousel-slide img-src="../assets/images/img-carousel3.png"></b-carousel-slide>
        <b-carousel-slide img-src="../assets/images/img-carousel4.png"></b-carousel-slide>
      </div>
    </b-carousel>
  </div>
</template>

<script>
export default {
  name: "Carousel",
  data() {},
};
</script>


<style>
.carousel {
  width: 100%;
  height: 80%;
}

.brand-carousel {
  color: black;
  position: absolute;
  top: 50%;
  transform: translateY(-65%);
  z-index: -1;
}
.carousel-inner {
}
@media (max-width: 360px) {
  .carousel-caption h3 {
    display: none;
  }
}
@media (max-width: 576px) {
  .brand-carousel {
    top: 40%;
    font-size: 10px;
  }
  .brand-carousel h1 {
    font-size: 80%;
  }
  b-button {
    font-size: 80%;
    margin-top: 0;
  }
}
@media (max-width: 768px) {
  .carousel-caption {
    top: 45%;
  }
  .carousel-caption h1 {
    font-size: 320%;
  }
  .carousel-caption h3 {
    font-size: 140%;
    font-weight: 400;
    padding-bottom: 0.2rem;
  }
  .carousel-caption .btn {
    font-size: 95%;
    padding: 8px 14px;
  }
  .display-4 {
    font-size: 200%;
  }
}
@media (min-width: 769px) {
  .brand-carousel {
    top: 40%;
    transform: translateY(-70%);
    margin-top: -90px;
    justify-content: center;
  }
}
@media (min-width: 1200px) {
  .carousel-inner {
    width: 100%;
    height: 100vh;
  }
  .brand-carousel {
    margin-top: -20%;
  }
}
</style>