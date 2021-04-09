<template>
  <div class="about">
    <b-container>
      <b-row>
        <div class="mx-auto">
        <h1>About</h1>
        </div>
      </b-row>

      <b-row class="form-group"></b-row>

      <b-row>
        <b-col cols="0" md="1"></b-col>
        <b-col cols="12" md="10">
          <p class="p-responsive">
            I grew up on the South Coast of NSW just outside of Bega. After I
            finished high school I moved to Wollongong (my friends were off to
            university there) and worked in various jobs for a few years. I have
            always had passion for IT and with some encouragement I finally
            took up study as a mature age student.<br /><br />
            I have just recently moved back to the South Coast and enjoy the
            peace and quite the country has to offer. In my spare time I enjoy
            gardening, keeping fit, working on various projects in the shed, photography and reading
            (sci-fi fan).
          </p>
        </b-col>
        <b-col cols="0" md="1"></b-col>
      </b-row>
      <!-- Spaceing -->
      <b-row class="form-group"></b-row>

  
      <b-row>
        <b-col cols="0" md="1"></b-col>
        <b-col cols="12" md="10">
          <img
            src="../assets/banner.jpg"
            class="img-fluid banner"
            alt="Sunrise over hills"
          />
        </b-col>
        <b-col cols="0" md="1"></b-col>
      </b-row>

      <b-row>
        <div class="mx-auto mt-3"> 
          <b-button target="_blank"
           class="link-out mr-2 custom-btn"
           href="https://www.instagram.com/jacks_nature_pics/?hl=en">
          Instagram Photography
          </b-button>
  
          <b-button target="_blank"
           class="link-out mr-2 custom-btn"
           href="https://www.instagram.com/jack_edwards_it/?hl=en">
          Instagram IT
          </b-button>

          <b-button target="_blank"
           class="link-out custom-btn"
           href="https://www.goodreads.com/user/show/86337535-jack">
          Goodreads Profile
          </b-button>
        </div>
      
      </b-row>
    </b-container>
  </div>
</template>

<script>

export default {
};
</script>


<style scoped>

.p-responsive{
  text-align: justify;
  color: white;
}
.banner {
  box-shadow: -5px 10px 10px rgba(0, 0, 0, 0.5);
}
</style>
