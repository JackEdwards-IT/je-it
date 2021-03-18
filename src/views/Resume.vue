<template>
  <div class="resume">
    <b-container>
      <b-row>
        <b-col cols="4"></b-col>
        <b-col cols="4"><h1 class="h1-responsive">Jack Edwards</h1></b-col>
        <b-col cols="4"></b-col>
      </b-row>

      <b-row class="form-group"></b-row>
      <b-row>
        <!-- DP & Education  -->
        <b-col cols="4">
          <img
            src="../assets/dp-70-cropped.png"
            class="img-fluid mb-2"
            alt="Jack profile picture"
          />
          <h2 class="h2-responsive">Education</h2>
          <p class="p-responsive education-title">
            Bachelor of Information Technolgy
          </p>
          <p class="p2-responsive">2018 - 2021</p>
          <p class="p2-responsive">Royal Melbourne Institute of Technology</p>
          <p class="p2-responsive">&#8594; Minoring in Web Design</p>
          <p class="p2-responsive">&#8594; Distinction Average</p>
        </b-col>

        <b-col cols="8">
          <p class="p-responsive" id="writeup">
            Strong focus on full stack web development with exposure to languages and platforms including Java, C, PHP, Node.js, Vue.js, PgSql & Wordpress. See the portfolio section for an
            overview of some of my projects and technologies I have used.
          </p>
          <b-row class="form-group"></b-row>
          <p class="p-responsive" id="writeup">
            I am ambitous and enjoy taking on new challenges, such as learning new languages and frameworks.
            The more I learn and expand my knowledge, the more flexible I become in solving problems. 
          </p>
          <b-row class="form-group"></b-row>
          <b-row class="form-group"></b-row>
          <p class="p-responsive" id="writeup">
            If you would like to see my full work history prior to IT studies
            see my LinkedIn profile.
          </p>
          <b-row class="form-group"></b-row>

          <b-button target="_blank"
           class="link-out mr-2 mt-1"
           variant="danger"
           href="https://au.linkedin.com/in/jse998">
          LinkedIn Profile
          </b-button>
        </b-col>
      </b-row>
      <b-row> </b-row>
    </b-container>
  </div>
</template>

<script>


export default {
};
</script>

<style scoped>
#writeup{ 
  text-align: justify;
}
.h1-responsive,
.h3-responsive {
  text-align: center;
}

p2 {
  font-family: "Titillium Web", sans-serif;
  color: lightgray;
  font-weight: 100;
  margin: 0;
}

p {
  margin-bottom: 0;
}
.education-title {
  color: #35a7ff;
}
</style>