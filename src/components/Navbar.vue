<template>
<b-container>
    <!-- NavBar -->
  <ul id="navigation">
    <nav class="navbar">
      <router-link to="/"><li>Home</li></router-link>
      <router-link to="resume"><li>Qualifications</li></router-link>
      <router-link to="portfolio"><li>Portfolio</li></router-link>
      <router-link to="about"><li>About</li></router-link>
      <router-link to="contact"><li>Contact</li></router-link>
    </nav>
  </ul>
  <!-- Hamburger -->

<div class="burger">
    <Slide 
    right 
    width="180"
    :closeOnNavigation="true">
      <router-link to="/"><li>Home</li></router-link>
      <router-link to="resume"><li>Qualifications</li></router-link>
      <router-link to="portfolio"><li>Portfolio</li></router-link>
      <router-link to="about"><li>About</li></router-link>
      <router-link to="contact"><li>Contact</li></router-link>
    </Slide>
</div>
  

</b-container>
</template>

<script>
import { Slide } from 'vue-burger-menu'
export default {
    components: {
        Slide
    }
};
</script>

<style scoped>
ul {
  position: relative;
  display: block;
}

li {
  display: inline;
  text-align: center;
  padding-right: 0vw;
  text-decoration: none;
  font-family: "Titillium Web", sans-serif;
  font-weight: 900;
  letter-spacing: 4px;
  color: #da4167;
  font-size: 20px;
  -moz-transition: all 0.2s ease-in;
  -o-transition: all 0.2s ease-in;
  -webkit-transition: all 0.2s ease-in;
  transition: all 0.2s ease-in;
}
@media only screen and (max-width: 768px) {
  li{
    font-size: 15px;
  }
}

li:hover,
#active-page {
  cursor: pointer;
  color: #35a7ff;
  text-shadow: 0px 0px 30px #35a7ff;
  -moz-transition: all 0.2s ease-in;
  -o-transition: all 0.2s ease-in;
  -webkit-transition: all 0.2s ease-in;
  transition: all 0.2s ease-in;
}
.router-link-exact-active > li {
  opacity: 1;
  text-decoration: none;
  color: #91cfff;
  text-shadow: 0px 0px 30px #b6df5d;
  /* OG shadow and text colour: #35A7FF  */
}

a,
a:link,
a:visited,
a:focus,
a:hover,
a:active {
  text-decoration: none !important;
}
.burger{
    display: none;
}
/* Media query  */
@media only screen and (max-width: 850px){
    .navbar{
        display: none;
    }
    .burger{
        display: inline;
    }
}
</style>

// Styling for burger menu
<style>
.bm-burger-button {
      z-index: 999;
      position: fixed !important;
      width: 36px !important;
      height: 30px !important;
      top: 10px !important;
      cursor: pointer;
      right: 10px !important;
    }
    .bm-burger-bars {
      background-color: #da4167 !important;
    }
    .line-style {
      position: absolute !important;
      height: 20% !important;
      left: 0 !important;
      right: 0 !important;
    }
    .cross-style {
      position: absolute !important;
      top: 12px !important;
      right: 2px !important;
      cursor: pointer !important;
    }
    .bm-cross {
      background: #da4167 !important;
    }
    .bm-cross-button {
      height: 24px !important;
      width: 24px !important;
    }
    .bm-menu {
      height: 100%; /* 100% Full-height */
      width: 0; /* 0 width - change this with JavaScript */
      position: fixed; /* Stay in place */
      z-index: 1000; /* Stay on top */
      top: 0;
      left: 0;
      background-color: rgb(63, 63, 65); /* Black*/
      overflow-x: hidden; /* Disable horizontal scroll */
      padding-top: 60px; /* Place content 60px from the top */
      transition: 0.5s; /*0.5 second transition effect to slide in the sidenav*/
    }

    .bm-overlay {
      background: rgba(0, 0, 0, 0.3);
    }
    .bm-item-list {
      color: #b8b7ad !important;
      margin-left: 5% !important;
      font-size: 20px  !important;
    }
    .bm-item-list > * {
      display: flex;
      text-decoration: none;
      padding: 0.7em;
    }
    .bm-item-list > * > span {
      margin-left: 10px;
      font-weight: 700;
      color: white;
    }
</style>