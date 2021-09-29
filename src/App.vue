<template>
  <div id="app">
   <div class="firstScreen"><div><Cube></Cube></div>
   <div class='videobutton'> <div><Video></Video></div><div><Button></Button></div></div></div>
   <div class='footer'><Footer></Footer></div>  </div>
</template>

<script>
import Button from './components/bannerButton.vue'
import Cube from './components/bannerCube.vue'
import Footer from './components/bannerFooter.vue'
import Video from './components/bannerVideo.vue'
export default {
  name: 'App',
  components: {
    Button,
    Cube,
    Footer,
    Video
  }
}
</script>

<style>
  @font-face {
     font-family: 'LeroyMerlinSans-Bold';
     src: url('/assets/fonts/LeroyMerlinSans-Bold.eot');
     src: url('/assets/fonts/LeroyMerlinSans-Bold?#iefix') format('embedded-opentype'),
     url('/assets/fonts/LeroyMerlinSans-Bold.otf') format('font-opentype'),
     url('/assets/fonts/LeroyMerlinSans-Bold.woff') format('font-woff'),
     url('/assets/fonts/LeroyMerlinSans-Bold.ttf') format('font-truetype');    
     font-weight: bold;
     font-style: bold;

     font-family: 'LeroyMerlinSans-Regular';
     src: url('/assets/fonts/LeroyMerlinSans-Regular.eot');
     src: url('/assets/fonts/LeroyMerlinSans-Regular?#iefix') format('embedded-opentype'),
     url('/assets/fonts/LeroyMerlinSans-Regular.otf') format('font-opentype'),
     url('/assets/fonts/LeroyMerlinSans-Regular.woff') format('font-woff'),
     url('/assets/fonts/LeroyMerlinSans-Regular.ttf') format('font-truetype');    
     font-weight: normal;
     font-style: normal;
      }
#app { 
    display: grid; 
    margin: 0;
    padding: 0;
    /* grid-template-columns: 57% 43%; */
     grid-template-rows: 760px 50px;
      height: 100vh; 
    /* grid-gap: 20px;
   
    /* position: relative; */
}
.firstScreen {
  display: grid;
  grid-template-columns: 1fr 1fr;
}
.footer {
  bottom: 0;
}

.videobutton{
  display: flex;
  flex-direction: column;
  /* margin-left: 2em; */
}

@media screen and (max-width: 980px) {
    #app{
        display: grid; 
        grid-template-columns: 1fr;
        min-height: 100vh;
    }
    .firstScreen {
       display: grid; 
       grid-template-columns: 1fr;
    }
}

</style>
