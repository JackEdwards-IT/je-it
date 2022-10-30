<template>
  <div class="resume">
    <b-container>
      <b-row>
        <div class="mx-auto">
          <h1>Jack Edwards</h1>
        </div>
      </b-row>

      <b-row class="form-group"></b-row>

      <!-- Education -->
      <b-row>
        <b-col cols="0" md="1"></b-col>

        <!-- RMIT -->
        <b-col cols="7" md="6">
          <h3>Education</h3>
          <p class="p-responsive education-title">
            Bachelor of Information Technology with Distinction
          </p>
          <p id="education-subtext" class="p2-responsive">2018 - 2021</p>
          <p id="education-subtext" class="p2-responsive">
            Royal Melbourne Institute of Technology
          </p>
          <p id="education-subtext" class="p2-responsive">&#8594; Minoring in Web Design</p>
        </b-col>
        <b-col cols="0" md="1"></b-col>

        <!-- DP -->
        <b-col cols="5" md="4">
          <img
            src="../assets/dp-70-cropped.png"
            class="img-fluid mb-2"
            alt="Jack profile picture"
          />
        </b-col>
      </b-row>

      <!-- Writeup -->
      <b-row>
        <b-col cols="0" md="1"></b-col>
        <b-col cols="12" md="10"
          ><hr />
          <p id="writeup">
           I currently work as a Javascript developer predominantly in the frontend for large eCommerce sites built on Nuxt.js.
          </p><p id="writeup" class="mt-3">
            My previous role as a graduate developer had me performing routine maintenance and incremental fixes on a 
            Java analytics backend, maintenance on client facing Angular/Java stacks and working with a Python based ETL pipeline 
            creating new scripts and troubleshooting data issues.
          </p>
          <p id="writeup" class="mt-3">
            Personally, I am eager and motivated to take on new challenges and
            refine and apply the technical skills I have learned within my
            degree and time spent as a graduate developer.
          </p>
        
          <p class="p-responsive mt-3" id="writeup">
            To view my full work history see my 
            <b-link
              target="_blank"
              href="https://au.linkedin.com/in/je-it"
              class="card-link white-link"
              >LinkedIn Profile.</b-link
            >
          </p>
          <b-row class="form-group"></b-row>
          <!-- <hr> -->
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
#writeup {
  text-align: justify;
  color: white;
}
.mobile-profile {
  display: none;
  color: white;
}
.h1-responsive,
.h3-responsive {
  text-align: center;
}

#education-subtext {
  font-family: "Titillium Web", sans-serif;
  color: white;
  font-weight: 100;
  margin: 0;
}

hr {
  height: 1px !important;
  background-color: rgba(161, 161, 161, 0.514) !important;
}
p {
  margin-bottom: 0;
}
.education-title {
  color: #35a7ff;
  font-size: 19px;
}
@media only screen and (max-width: 767px) {
  .md-profile {
    display: none;
  }
  .mobile-profile {
    display: inline-flex;
  }
}
.white-link {
  color: #99d3f4 !important;
  text-decoration: underline !important;
}
</style>