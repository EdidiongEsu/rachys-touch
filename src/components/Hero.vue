<template>
  <div class="carousel">
    <b-carousel
      id="carousel-fade"
      style="text-shadow: 0px 0px 2px #000"
      fade
      controls
      interval="3000"
    >
      <div class="carousel-inner max-vh-100">
        <b-carousel-slide caption="First slide" img-src="../assets/images/img-carousel1.png"></b-carousel-slide>
        <b-carousel-slide caption="Second Slide" img-src="../assets/images/img-carousel2.png"></b-carousel-slide>
        <b-carousel-slide caption="Third Slide" img-src="../assets/images/img-carousel3.png"></b-carousel-slide>
        <b-carousel-slide caption="Fourth Slide" img-src="../assets/images/img-carousel4.png"></b-carousel-slide>
      </div>
    </b-carousel>
  </div>
</template>

<script>
export default {
  name: "Hero",
  data() {},
};
</script>


<style>
.carousel {
  width: 100%;
  overflow: hidden;
  height: 610px;
}
caption {
  font-size: 100px;
  display: block;
}
</style>