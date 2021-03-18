<template>
  <div class="contact">
    <b-container>
      <b-row>
        <b-col cols="4"></b-col>
        <b-col cols=""><h1 class="h1-responsive">Contact</h1></b-col>
        <b-col cols="4"></b-col>
      </b-row>

      <b-row class="form-group"></b-row>
      <b-row>
        <b-col cols="2"></b-col>

        <b-col cols="8">
          <b-form
            :model="form"
            @submit.prevent="submit"
            ref="contactForm"
            action="https://formspree.io/f/mjvpnqep"
            method="POST"
          >
            <b-form-input
              type="text"
              placeholder="Enter your name"
              required
            ></b-form-input>
            <b-form-input
              type="email"
              placeholder="Enter email"
              required
            ></b-form-input>
            <b-form-textarea
              rows="3"
              max-rows="10"
              placeholder="Enter your message"
              required
            ></b-form-textarea>

            <div class="form-group row">
              <label for="robot" class="col-sm-2 col-form-label"></label>
              <div class="col-sm-10">
                <vue-recaptcha
                  ref="recaptcha"
                  @verify="onVerify"
                  sitekey="6LexGYQaAAAAAE8UsVFh8COeUN1GNCmDNPXqP0uL"
                >
                </vue-recaptcha>
              </div>
            </div>
            <b-button type="submit" variant="primary">Send</b-button>.
          </b-form>
        </b-col>

        <b-col cols="2"></b-col>
      </b-row>
    </b-container>
  </div>
</template>


<script>
import VueRecaptcha from "vue-recaptcha";

export default {
  data() {
    return {
      form: {
        robot: false,
      },
    };
  },
  methods: {
    submit: function () {
      if (this.form.robot) {
        console.log("test");
      }
    },
    onVerify: function (response) {
      if (response) this.form.robot = true;
    },
  },
  components: { VueRecaptcha },
};
</script>

<style scoped>
.h1-responsive {
  text-align: center;
}
.p-responsive {
  font-size: calc(50% + 0.4vw + 0.4vh);
}
p {
  margin-bottom: 0;
}
</style>