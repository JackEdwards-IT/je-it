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
            Bachelor of Information Technology
          </p>
          <p id="education-subtext" class="p2-responsive">2018 - 2021</p>
          <p id="education-subtext" class="p2-responsive">
            Royal Melbourne Institute of Technology
          </p>
          <!-- <p id="education-subtext" class="p2-responsive">&#8594; Minoring in Web Design</p>
          <p id="education-subtext" class="p2-responsive">&#8594; Distinction Average</p> -->
          <!-- CSU -->
          <p class="p-responsive education-title mt-2">
            Graduate Certificate in Cloud Computing and Virtualisation
          </p>
          <p id="education-subtext" class="p2-responsive">2021 - Ongoing</p>
          <p id="education-subtext" class="p2-responsive">
            Charles Sturt University
          </p>
          <!-- <p id="education-subtext" class="p2-responsive">&#8594; </p>
          <p id="education-subtext" class="p2-responsive">&#8594; Distinction Average</p> -->
        </b-col>
        <b-col cols="0" md="1"></b-col>

        <!-- DP -->
        <b-col cols="5" md="4">
          <img
            src="../assets/dp-70.png"
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
            Interested in full stack web development as well as all aspects of
            IT. With exposure to multiple languages and platforms such as Java,
            C, Node.js, Vue.js, PgSql. See the portfolio section for an overview
            of some of my projects and the technologies I have used.
          </p>
          <b-row class="form-group"></b-row>
          <p id="writeup">
            I am ambitious and enjoy taking on new challenges and learning
            opportunities. While I have a focus on web dev through my minor, I
            am open to all areas of the industry. I have recently started part
            time studies in a Graduate Certificate in Cloud Computing and
            Virtualisation.
          </p>

          <b-row class="form-group"></b-row>
          <p class="p-responsive" id="writeup">
            If you would like to see my full work history prior to IT studies
            see my
            <b-link
              target="_blank"
              href="https://au.linkedin.com/in/je-it"
              class="card-link"
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
}
@media only screen and (max-width: 767px) {
  .md-profile {
    display: none;
  }
  .mobile-profile {
    display: inline-flex;
  }
}
</style>