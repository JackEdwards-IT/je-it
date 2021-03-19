<template>
  <div class="contact">
    <b-container>
      <b-row>
        <b-col cols="4"></b-col>
        <b-col cols=""><h1 class="h1-responsive">Contact</h1></b-col>
        <b-col cols="4"></b-col>
      </b-row>

      <b-row>
        <b-col cols="2"></b-col>

        <b-col cols="8">
          <b-form class="contact-form" @submit.prevent="sendEmail">
            <b-form-group
              id="input-group-1"
              label="Email Address:"
              label-for="input-1"
            >
              <b-form-input
                id="input-1"
                type="email"
                name="from_email"
                placeholder="Enter Email"
                required
              >
              </b-form-input>
            </b-form-group>

            <b-form-group
              id="input-group-2"
              label="Your Name:"
              label-for="input-2"
            >
              <b-form-input
                id="input-2"
                name="from_name"
                placeholder="Enter name"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group
              id="input-group-3"
              label="Please enter your message:"
              label-for="input-3"
            >
              <b-form-textarea
                id="input-3"
                placeholder="Enter Message"
                required
                name="message"
                rows="4"
                max-rows="7"
              ></b-form-textarea>
            </b-form-group>
            >
            <!-- Recaptcha Checkbox -->
            <div class="g-recaptcha" data-sitekey="6LexGYQaAAAAAE8UsVFh8COeUN1GNCmDNPXqP0uL"></div>
            <b-button variant="success" type="submit" value="Send"
              >Send</b-button
            >
          </b-form>
          <!-- Indicate success or failure of form submission -->
          <div
            class="alert alert-success mt-2"
            role="alert"
            v-show="messageSent"
          >
            Message successfully sent. I will be in touch shortly.
          </div>

          <div
            class="alert alert-danger mt-2"
            role="alert"
            v-show="messageNotSent"
          >
            Something went wrong. Please contact me directly: jack at je-it dot
            com.
          </div>
        </b-col>

        <b-col cols="2"></b-col>
      </b-row>
    </b-container>
  </div>
</template>


<script>
import emailjs from "emailjs-com";

export default {
  data() {
    return {
      messageNotSent: true,
      messageSent: false,
    };
  },
  methods: {
    sendEmail: (e) => {
      emailjs
        .sendForm(
          "service_3jfiw2l",
          "template_d9zorsq",
          e.target,
          "user_ToFE396KP3LoLIYBpk92K"
        )
        .then(
          () => {
            // console.log("SUCCESS!", result.status, result.text);
            this.messageSent = true;
          },
          () => {
            // console.log("FAILED...", error);
            this.messageNotSent = true;
          }
        );
    },
  },
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