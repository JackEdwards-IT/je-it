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

      
          <h2 class="h2-responsive">
            <form action="https://formspree.io/f/mjvpnqep" method="POST">
              <div class="g-recaptcha" data-sitekey="6LexGYQaAAAAAE8UsVFh8COeUN1GNCmDNPXqP0uL"></div>
              <label>
                Your email:
                <input type="email" name="_replyto" />
              </label>
              <label>
                Your message:
                <textarea name="message"></textarea>
              </label>

              <!-- your other form fields go here -->

              <button type="submit">Send</button>
            </form>
            
          </h2></b-col>

          <b-col cols="2"></b-col>

      </b-row>
    </b-container>
  </div>
</template>

<script src="https://www.google.com/recaptcha/api.js" async defer></script>

<script>
export default {};
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