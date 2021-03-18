<template>
  <div class="resume">
    <b-container>
      <b-row>
        <b-col></b-col>
        <b-col cols="10"><h1 class="h1-responsive">Jack Edwards</h1></b-col>
        <b-col></b-col>
      </b-row>

      <b-row class="form-group"></b-row>
      <b-row>
        <b-col cols="4">
          <img
            src="../assets/dp-70.png"
            class="img-fluid"
            alt="Jack profile picture"
          />

          <h2 class="h2-responsive">Education</h2>
          <p class="p-responsive education-title">
            Bachelor of Information Technolgy
          </p>
          <p class="p2-responsive">2018 - 2021</p>
          <p class="p2-responsive">Royal Melbourne Institute of Tehnology</p>
          <p class="p2-responsive">&#8594; Minoring in Web Design</p>
        </b-col>
        <b-col cols="7">
          <p class="p-responsive">
            Strong focus on full stack web development with exposure to numerous
            other languages and technologies. See the portfolio section for an
            overview of some of my projects.
          </p>
          <b-row class="form-group"></b-row>
          <p class="p-responsive">
            I enjoy taking on new challenges and the endless learning
            opportunites IT has to offer.
          </p>
          <b-row class="form-group"></b-row>
          <b-row class="form-group"></b-row>
          <p class="p-responsive">
            If you would like to see my full work history prior to IT studies
            see my LinkedIn profile
          </p>
          <b-row class="form-group"></b-row>
          <a
            class="btn btn-outline-light link-out"
            href="https://au.linkedin.com/in/jse998"
            role="button"
            target="_blank"
            >LinkedIn Profile</a
          >
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