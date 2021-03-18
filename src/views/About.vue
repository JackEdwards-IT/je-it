<template>
  <div class="about">
    <b-container>
      
      <b-row>
        <b-col cols="5"></b-col>
        <b-col cols="2"><h1>About</h1></b-col>
        <b-col cols="5"></b-col>
      </b-row>

      <b-row class="form-group"></b-row>

      <b-row>
        <b-col cols="1"></b-col>
        <b-col cols="10">
          <p class="p-responsive">
            I grew up on the South Coast of NSW just outside of Bega, after I
            finished high school I moved to Wollongong (my friends were off to
            university there) and worked in various jobs for a few years. I have
            always had passion for IT and with a bit of encouragement I finally
            took up study as a mature age student.<br /><br />
            I have just recently moved back to the South Coast and enjoy the
            peace and quite the country has to offer. In my spare time I enjoy
            gardening, growing vegetables and herbs, keeping fit, working on
            various projects in the shed. I also enjoy photography and reading
            (sci-fi tragic!).
          </p>
        </b-col>
        <b-col cols="1"></b-col>
      </b-row>
      <!-- Spaceing -->
      <b-row class="form-group"></b-row>

  
      <b-row>
        <b-col cols="1"></b-col>
        <b-col cols="10">
          <img
            src="../assets/banner.jpg"
            class="img-fluid banner"
            alt="Sunrise over hills"
          />
        </b-col>
        <b-col cols="1"></b-col>
      </b-row>

      <b-row>
        
        <b-col cols="4"></b-col>
        <b-col cols="6">
  
          <b-button target="_blank"
           class="link-out mr-2 mt-1"
           variant="danger"
           href="https://www.instagram.com/jacks_nature_pics/?hl=en">
          Instagram Photos
          </b-button>
  
          <b-button target="_blank"
           class="link-out mt-1"
           variant="danger"
           href="https://www.goodreads.com/user/show/86337535-jack">
          Goodreads Profile
          </b-button>
        </b-col>
        
      </b-row>
    </b-container>
  </div>
</template>

<script>

export default {
};
</script>


<style scoped>

/* .link-out{
  margin: 4px 2px 0 2px;
  letter-spacing: 0.5px;
} */
.p-responsive{
  text-align: justify;
}
.banner {
  box-shadow: -5px 10px 10px rgba(0, 0, 0, 0.5);
}
</style>
