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
            I grew up on a small hobby farm near Bega on the Far South Coast of
            NSW. Eager to explore bigger cities, I moved to Wollongong and
            worked in the retail sector after highschool.</p>
            <p class="p-responsive mt-3">
            I have always had a
            passion for IT, and after some encouragement, I enrolled in an
            online Bachelor of Information Technology with the Royal Melbourne
            Institute of Technology as a mature aged student.</p>
            <p class="p-responsive mt-3">
            Returning to the
            country, I have recently moved back to the Bega Valley area, and am
            enjoying the ease of finding a parking space when I go grocery
            shopping. In my spare time I enjoy gardening, fitness, photography,
            reading, and creating an endless cycle of new mechanical and IT
            projects. 
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
        <b-col cols="0" md="1"></b-col>
        <b-col cols="12" md="10">
          <div class="mx-auto mt-3">
            <b-button
              target="_blank"
              class="link-out mr-2 mt-2 custom-btn"
              href="https://www.instagram.com/jacks_nature_pics/?hl=en"
            >
              Instagram Photography
            </b-button>

            <b-button
              target="_blank"
              class="link-out mr-2 mt-2 custom-btn"
              href="https://www.instagram.com/jack_edwards_it/?hl=en"
            >
              Instagram IT
            </b-button>

            <b-button
              target="_blank"
              class="link-out mt-2 custom-btn"
              href="https://www.goodreads.com/user/show/86337535-jack"
            >
              Goodreads Profile
            </b-button>
          </div>
        </b-col>
        <b-col cols="0" md="1"></b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {};
</script>


<style scoped>
.p-responsive {
  text-align: justify;
  color: white;
}
.banner {
  box-shadow: -5px 10px 10px rgba(0, 0, 0, 0.5);
}
</style>
