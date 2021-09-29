
<template>
<div class='wrapper'>
<swiper :effect="'cube'" :grabCursor="true" :cubeEffect='{
  "shadow": true,
  "slideShadows": true,
  "shadowOffset": 20,
  "shadowScale": 0.94
}' 
:autoplay='{
  "delay": 5000
}'
:pagination="false" class="mySwiper">
  <swiper-slide><img src="../assets/i/01.jpg" /></swiper-slide>
  <swiper-slide><img src="../assets/i/02.jpg" /></swiper-slide>
  <swiper-slide><img src="../assets/i/03.jpg" /></swiper-slide>
 
  </swiper>
  </div>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

import "swiper/swiper-bundle.min.css";

// import "swiper/effect-cube"
// import "swiper/pagination"


import "swiper/components/effect-cube/effect-cube.min.css";


// import './style.css';


// import Swiper core and required modules
import SwiperCore, {
  EffectCube
} from 'swiper';

// install Swiper modules
SwiperCore.use([EffectCube]);


export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {        
        
    };
  },
  methods: {
    
  }
  
}




</script>
<style>
#app { height: 100% }
html,
body {
  position: relative;
  height: 100%;
}

body {
  background: #eee;
  /* font-family: Helvetica Neue, Helvetica, Arial, sans-serif; */
  font-size: 14px;
  color: #000;
  margin: 0;
  padding: 0;
}

.swiper {
  width: 300px;
  height: 300px;
  position: absolute;
  /* left: 50%;
  top: 50%;
  margin-left: -150px;
  margin-top: -150px; */
}

.swiper-slide {
  background-position: center;
  background-size: cover;
}

.swiper-slide img {
  display: block;
  width: 100%;
}
.wrapper {
    position: relative;
    width: 640px;
    margin-left: 110px;
    margin-top: 60px;
}


@media screen and (max-width: 980px) {
  
.wrapper {
   
    width: 360px;
   
}
}
</style>