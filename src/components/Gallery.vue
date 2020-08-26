<template>
  <b-container fluid class="p-4 gallery text-center">
    <b-row class="justify-content-center pb-3">
      <h2>GALLERY</h2>
    </b-row>
    <b-row align-h="center gallery-inner">
      <b-col class="mr-n4 mb-4 gallery-col1 rounded-circle">
        <b-img thumbnail fluid :src="item" alt="Image 1"></b-img>
        <b-img class="rounded-circle" thumbnail fluid :src="item" alt="Image 1"></b-img>
        <b-img thumbnail fluid :src="item" alt="Image 1"></b-img>
      </b-col>
      <b-col>
        <b-img class="rounded-circle" thumbnail fluid :src="item" alt="Image 2"></b-img>
        <b-img thumbnail fluid :src="item" alt="Image 2"></b-img>
        <b-img class="rounded-circle" thumbnail fluid :src="item" alt="Image 2"></b-img>
      </b-col>
      <b-col class="ml-n4 mb-4 gallery-col3">
        <b-img thumbnail fluid :src="item" alt="Image 3"></b-img>
        <b-img class="rounded-circle" thumbnail fluid :src="item" alt="Image 3"></b-img>
        <b-img thumbnail fluid :src="item" alt="Image 3"></b-img>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "Gallery",
  data() {
    return {
      item: require("@/assets/images/gallery-image1.png"),
    };
  },
};
</script>


<style>
.gallery {
  background: rgba(212, 210, 210, 0.89);
}
@media (min-width: 768px) {
  .gallery-inner {
    justify-content: center !important;
  }
  .gallery-col1 {
    margin-right: -70px !important;
  }
  .gallery-col3 {
    margin-left: -70px !important;
  }
}
@media (min-width: 1000px) {
  .gallery-col1 {
    margin-right: -90px !important;
  }
  .gallery-col3 {
    margin-left: -90px !important;
  }
}
</style>