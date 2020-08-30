<template>
  <b-container fluid class="p-5 about-wrapper justify-content-center">
    <div class="about-content">
      <b-row class="justify-content-center pb-3">
        <h2>OUR SERVICES</h2>
      </b-row>
      <b-row>
        <b-col v-for="item in items" :key="item.id" class="col-12 text-center" md="4">
          <b-card
            :title="item.title"
            :img-src="item.image"
            img-top
            class="m-2 rounded"
            border-variant="dark"
          >
            <b-card-text>{{ item.text }}</b-card-text>
          </b-card>
        </b-col>
      </b-row>
    </div>
  </b-container>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      items: [
        {
          id: 1,
          title: "Facial Makeup",
          image: require("@/assets/images/card-image1.png"),
          text:
            "We highlight the beauty of our muses to bring out their facial exuberance.",
        },
        {
          id: 2,
          title: "Skin Care",
          image: require("@/assets/images/card-image2.png"),
          text:
            "We offer skin care advice to our clients depending on their skin type based on proven steps.",
        },
        {
          id: 3,
          title: "Trainings",
          image: require("@/assets/images/card-image3.png"),
          text:
            "We teach a wide range of skin-related topics which extends to head gear wears amd hoe to tie them. ",
        },
      ],
    };
  },
};
</script>


<style>
h2 {
  font-family: "Niconne", cursive;
}
</style>