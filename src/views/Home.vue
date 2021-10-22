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
            <b-col md="10"><h1>I'm <span id="red-text">J</span>ack <span id="red-text">E</span>dwards,</h1></b-col>
            <b-col></b-col>
         </b-row>
         <b-row>
           <b-col></b-col>
            <b-col md="10"><h1><span id="red-text">IT </span>Professional</h1></b-col>
            <b-col></b-col>
          </b-row>
          <b-row class="form-group"></b-row>
          <b-row>
            <b-col></b-col>
           <b-col md="10"> <h2 class="h2-responsive">Currently working as a full stack developer in an environment that uses Java, Angular, Postgres and Python</h2></b-col>
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

#red-text{
  color:red;
}

</style>