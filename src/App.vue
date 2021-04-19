<template>
  <div id="app">
    <navbar v-show="showNavBar"></navbar>

    <transition
      name="fade"
      mode="out-in"
      @beforeLeave="beforeLeave"
      @enter="enter"
      @afterEnter="afterEnter"
      >
      <router-view/>
    </transition>
  </div>
</template> 

<script>
import Navbar from "@/components/Navbar.vue";

export default {
  name: 'App',
  computed: {
    showNavBar(){
      if (this.$route.path === "/"){
        return false;
      } else {
        return true;
      }
    }
  },
  data(){
    return {
      prevHeight: 0,
    };
  },
  methods: {
    beforeLeave(element){
      this.prevHeight = getComputedStyle(element).height;
    },
    enter(element){
      const {height} = getComputedStyle(element);

      element.style.height = this.prevHeight;

      setTimeout(() => {
        element.style.height = height;
      });
    },
    afterEnter(element) {
      element.style.height = 'auto';
    },
  },
  components: { navbar: Navbar },
};
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

@import url('https://fonts.googleapis.com/css2?family=Titillium+Web&display=swap');

html,
body {
    background-color: #1D1D1D !important;
}
 .fade-enter-active,
 .fade-leave-active {
   transition-duration: 0.0s;
   transition-property: opacity;
   transition-property: height, opacity;
   transition-timing-function: ease;
   overflow: hidden;
 }
.fade-enter,
.fade-leave-active {
  opacity: 0
}

/*Fonts*/


h1 {
    font-family: 'Titillium Web', sans-serif;
    color: white;
    letter-spacing: 1px;
}

h2{
    font-family: 'Titillium Web', sans-serif;
    color: white;
}
h3{
    font-family: 'Titillium Web', sans-serif;
    color: white;
}

p {
   font-family: 'Titillium Web', sans-serif;
   font-size: 18px;
}



/* Overide some of the bootstrap button styling */
.custom-btn{
  background-color: rgba(0, 0, 0, 0.205) !important;
  color: white !important;
  border-color: black !important;
  border-radius: 5px !important;
  border-width: 1px !important;
  letter-spacing: 1px;
  font-family: 'Titillium Web', sans-serif !important;
  font-weight: 600 !important;
}

.custom-btn:hover {
  cursor: pointer;
  color:#35a7ff !important;
  border-color: black !important;
  -moz-transition: all 0.2s ease-in;
  -o-transition: all 0.2s ease-in;
  -webkit-transition: all 0.2s ease-in;
  transition: all 0.2s ease-in;
}

.form-lbl {
  color: white !important;
  font-family: 'Titillium Web', sans-serif !important;
}

</style>
