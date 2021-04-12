<template>
  
    <div class="home">
        <b-container>
          <b-row class="form-group"></b-row>
         <b-row>
           <b-col></b-col>
            <b-col md="10"><h1 class="h1-responsive">Hi,</h1></b-col>
            <b-col></b-col>
         </b-row>
         <b-row>
           <b-col></b-col>
            <b-col md="10"><h1 v-lettering class="firstLine h1-responsive">I'm Jack Edwards,</h1></b-col>
            <b-col></b-col>
         </b-row>
         <b-row>
           <b-col></b-col>
            <b-col md="10"><h1><span class="it">IT </span>student graduating in 2021.</h1></b-col>
            <b-col></b-col>
          </b-row>
          <b-row class="form-group"></b-row>
          <b-row>
            <b-col></b-col>
           <b-col md="10"> <h2 class="h2-responsive">Developing skills in full stack web development, cloud platforms, Java programming and building IOT projects in my spare time.</h2></b-col>
          <b-col></b-col>
          </b-row>

          <b-row>
            <b-col></b-col>
           <b-col md="10">
             <ul id="navigation">
                <router-link to="resume"><li class="menu-text">Qualifications</li></router-link>
                <router-link to="portfolio"><li class="menu-text">Portfolio</li></router-link>
                <router-link to="about"><li class="menu-text">About</li></router-link>
                <router-link to="contact"><li class="menu-text">Contact</li></router-link>
            </ul>
            </b-col>
          <b-col></b-col>
          </b-row>
        </b-container>
    </div>
        
</template>

<script>

export default {
  name: 'Home',
}
</script>

<style>
/*Individual lettering colours, using v-lettering*/
 .firstLine .vl--i-5, .firstLine .vl--i-10{ 
    color: red;
}
 .secondLine .vl--i-1, .secondLine .vl--i-2{ 
    color: red;
}

li {
    display: inline;
    text-align: center;
    padding-right: 2vw;
    text-decoration: none; 
    font-family: 'Titillium Web', sans-serif; 
    font-weight: 900;
    letter-spacing: 4px;
    font-size: 25px;
    color: #DA4167;
    -moz-transition: all 0.2s ease-in;
    -o-transition: all 0.2s ease-in;
    -webkit-transition: all 0.2s ease-in;
    transition: all 0.2s ease-in;
}

li:hover,
#active-page {
    cursor: pointer;
    color: #35A7FF;
    text-shadow:0px 0px 30px #35A7FF;
    -moz-transition: all 0.2s ease-in;
    -o-transition: all 0.2s ease-in;
    -webkit-transition: all 0.2s ease-in;
    transition: all 0.2s ease-in;
}
.router-link-active,
.router-link-exact-active {
  text-decoration: none;
  color: #000;
}

a, a:link, a:visited, a:focus, a:hover, a:active{
  text-decoration:none !important;
}
</style>

<style scoped>
  @media only screen and (max-width: 768px) {
  #navigation{
    padding-top: 10px;
  }
  li{
    display: flex;
    padding-right: 0px;
  }
  ul {
    /* Overide user agent styles for menu padding */
    margin-block-start: 0px;
    padding-inline-start: 0px;
  }
}

.it{
  color:red;
}

</style>