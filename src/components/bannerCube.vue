<template>
<div class='wrapper'>
<swiper :effect="'cube'" :grabCursor="true" :cubeEffect='{
  "shadow": true,
  "slideShadows": true,
  "shadowOffset": 20,
  "shadowScale": 0.94
}' 
:autoplay='{
   delay: 5000
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
import "swiper/swiper-bundle.min.js";

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
    //  loop: true,
    // speed: 4000,
    // autoplay: {
    // enabled: true,
    // delay: 2,}
  }
}

// const swiper = new Swiper('.mySwiper', {
//  autoplay: {
//    delay: 5000,
//  },
// });

</script>
<style>
#app { height: 100% }
html,
body {
  position: relative;
  height: 100%;
}

body {
  margin: 0;
  padding: 0;
}

.swiper {
  width: 300px;
  height: 300px;
  position: absolute;
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
    margin-top: 2em;
}


@media screen and (max-width: 980px) {  
.wrapper {   
    width: 360px;
}
}
</style>