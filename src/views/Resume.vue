<template>
  <div class="resume">
    <b-container>
      <b-row>
        <div class="mx-auto">
          <h1>Jack Edwards</h1>
        </div>
      </b-row>

      <b-row class="form-group"></b-row>
      <b-row>
        <!-- DP & Education Desktop View -->
        <b-col cols="0" md="4" class="md-profile">
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

        <!-- Writeup -->

        <b-col cols="12" md="8">
          <p class="p-responsive" id="writeup">
            Strong focus on full stack web development with exposure to
            languages and platforms including Java, C, PHP, Node.js, Vue.js,
            PgSql & Wordpress. See the portfolio section for an overview of some
            of my projects and technologies I have used.
          </p>
          <b-row class="form-group"></b-row>
          <p class="p-responsive" id="writeup">
            I am ambitous and enjoy taking on new challenges, such as learning
            new languages and frameworks. The more I learn and expand my
            knowledge, the more flexible I become in solving problems.
          </p>

          <b-row class="form-group"></b-row>
          <p class="p-responsive" id="writeup">
            If you would like to see my full work history prior to IT studies
            see my LinkedIn profile.
          </p>
          <b-row class="form-group"></b-row>

          <!-- DP & Education Mobile View -->
          <b-row class="mobile-profile">
          <b-col cols="5">
            <img
              src="../assets/dp-70-cropped.png"
              class="img-fluid mb-2"
              alt="Jack profile picture"
            />
          </b-col>
          <b-col cols="7">
            <h2 class="h2-responsive">Education</h2>
            <p class="education-title">
              Bachelor of Information Technolgy
            </p>
            <p>2018 - 2021</p>
            <p>Royal Melbourne Institute of Technology</p>
            <p>&#8594; Minoring in Web Design</p>
            <p>&#8594; Distinction Average</p>
          </b-col>
          </b-row>

          <b-button
            target="_blank"
            class="link-out mr-2 mt-1"
            variant="danger"
            href="https://au.linkedin.com/in/jse998"
          >
            LinkedIn Profile
          </b-button>
        </b-col>
      </b-row>
      <b-row> </b-row>
    </b-container>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#writeup {
  text-align: justify;
}
.mobile-profile{
  display: none;
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
@media only screen and (max-width: 768px) {
  .md-profile {
    display: none;
  }
  .mobile-profile {
    display:inline-flex;
  }
}
</style>