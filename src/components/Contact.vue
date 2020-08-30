<template>
  <b-container id="contact">
    <b-row class="justify-content-center p-3">
      <h2>Book a session with Us!</h2>
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
          <b-form-datepicker id="example-datepicker" v-model="value" class="mb-2"></b-form-datepicker>
        </div>

        <div>
          <label for="example-timepicker">Choose preferred start time</label>
          <b-form-timepicker locale="en"></b-form-timepicker>
        </div>

        <b-button type="submit" class="m-2" variant="primary">Submit</b-button>
        <b-button type="reset" class="m-2" variant="danger">Reset</b-button>
      </b-form>
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
      },
      show: true,
      value: "",
    };
  },
  methods: {
    onSubmit(evt) {
      evt.preventDefault();
      alert(JSON.stringify(this.form));
    },
    onReset(evt) {
      evt.preventDefault();
      // Reset our form values
      this.form.email = "";
      this.form.name = "";
      // Trick to reset/clear native browser form validation state
      this.show = false;
      this.$nextTick(() => {
        this.show = true;
      });
    },
  },
};
</script>

<style></style>
