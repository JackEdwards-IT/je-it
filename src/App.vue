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
  // props: {
  //   showNavBar: Boolean,
  // },
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
.App__footer {
  color: white;
}

/*Fonts*/
h1 {
    font-family: 'Titillium Web', sans-serif;
    color: white;
    letter-spacing: 1px;
}
h2{
    font-family: 'Titillium Web', sans-serif;
    color: lightgray;
}
p {
  font-family: 'Titillium Web', sans-serif;
  color: lightgray;
}
.h1-responsive,
.firstLine,
.secondLine {
  font-size: calc(70% + 1vw + 1vh);
}
.h2-responsive {
  font-size: calc(50% + 0.7vw + 0.7vh);
}
.menu-text {
  font-size: calc(50% + 0.6vw + 0.6vh);
  padding-right: 4vw;
}
.p-responsive {
   font-size: calc(50% + 0.5vw + 0.5vh);
}


</style>
