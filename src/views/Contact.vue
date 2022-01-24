<template>
  <div class="contact">
    <b-container>
      <b-row>
        <div class="mx-auto">
        <h1>Contact</h1>
        </div>
      </b-row>

      <b-row>
       <div class="mx-auto">
          <p class="p-responsive">Please email me at: <font color=#35a7ff>Jack@je-it.com</font></p>
       </div>      
      </b-row>

      <!-- <b-row>
        <b-col cols="0" md="2"></b-col>

        <b-col cols="12" md="8">
          <b-form ref="form" class="contact-form" @submit.prevent="sendEmail">
            <b-form-group
              id="input-group-1"
              label-class="form-lbl"
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
              label-class="form-lbl"
              label="Your Name:"
              label-for="input-2"
            >
              <b-form-input
                id="input-2"
                name="from_name"
                placeholder="Enter Name"
                required
              ></b-form-input>
            </b-form-group>

            <b-form-group
              id="input-group-3"
              label-class="form-lbl"
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
           

            TODO remove hardcoding of submit state to reflect response from emailJS API 

            <b-button :disabled="submitDisabled" @click="changeStates(true)" @clik="sendEmail()" class="custom-btn" type="submit" value="Send"
              >Send</b-button
            >

 
          </b-form>
          Indicate success or failure of form submission
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

        <b-col cols="0" md="2"></b-col>
      </b-row> --> 
    </b-container>
  </div>
</template>


<script>
import emailjs from "emailjs-com";

export default {
  data() {
    return {
      submitDisabled: false,
      messageNotSent: false,
      messageSent: false,
    };
  },
  methods: {
    sendEmail() {
      console.log("send email...")
      emailjs.sendForm('service_3jfiw2l', 'template_d9zorsq', this.$refs.form, 'user_ToFE396KP3LoLIYBpk92K')
        .then((result) => {
            console.log('SUCCESS!', result.text);
        }, (error) => {
            console.log('FAILED...', error.text);
        });
    },
    
    changeStates(outcome){
      if(outcome){
        this.messageSent = true;
        this.submitDisabled = true;
      } else {
        this.messageNotSent = true;
        this.submitDisabled = true;
      }

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
  text-align: justify;
  color: white;
}
p {
  margin-bottom: 0;
}

</style>