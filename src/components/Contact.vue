<template>
  <b-container id="contact">
    <b-row class="justify-content-center p-3">
      <h2>BOOK A SESSION WITH US!</h2>
    </b-row>
    <div>
      <b-form @submit="onSubmit" @reset="onReset" v-if="show">
        <b-form-group id="input-group-1" label="Email address:" label-for="input-1">
          <b-form-input
            id="input-1"
            v-model="form.email"
            type="email"
            required
            placeholder="Enter email"
          ></b-form-input>
        </b-form-group>

        <b-form-group id="input-group-2" label="Your Name:" label-for="input-2">
          <b-form-input id="input-2" v-model="form.name" required placeholder="Enter name"></b-form-input>
        </b-form-group>

        <div>
          <label for="example-datepicker">Choose a date</label>
          <b-form-datepicker id="example-datepicker" v-model="form.date" class="mb-2"></b-form-datepicker>
        </div>

        <div>
          <label for="example-timepicker">Choose preferred start time</label>
          <b-form-timepicker locale="en" v-model="form.time"></b-form-timepicker>
        </div>

        <b-button type="submit" class="m-2" variant="primary">Submit</b-button>
        <b-button type="reset" class="m-2" variant="danger">Reset</b-button>
      </b-form>
    </div>
    <div class="googlemaps py-2">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2810.997448489098!2d6.981312613315423!3d4.880796622366953!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x1069d1bf2996ff89%3A0xf33d84edbb18599f!2sRumuagholu%20state%20Secondary%20school!5e0!3m2!1sen!2sng!4v1598758574566!5m2!1sen!2sng"
        width="100%"
        height="300"
      ></iframe>
    </div>
  </b-container>
</template>

<script>
export default {
  name: "Contact",
  data() {
    return {
      form: {
        email: "",
        name: "",
        date: "",
        time: "",
      },
      show: true,
    };
  },
  methods: {
    onSubmit(evt) {
      evt.preventDefault();
      // console.log(JSON.stringify(this.form));
      // alert(JSON.stringify(this.form));
      this.onReset(evt);
    },
    onReset(evt) {
      evt.preventDefault();
      // Reset our form values
      this.form.email = "";
      this.form.name = "";
      this.form.date = "";
      this.form.time = "";
      // Trick to reset/clear native browser form validation state
      this.show = false;
      this.$nextTick(() => {
        this.show = true;
      });
    },
  },
};
</script>

<style>
</style>
