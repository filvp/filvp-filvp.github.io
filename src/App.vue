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
    font-family: 'Leroy Merlin Sans';
    src: url('./assets/fonts/LeroyMerlinSans-Bold.eot');
    src: url('./assets/fonts/LeroyMerlinSans-Bold.eot?#iefix') format('embedded-opentype'),
        url('./assets/fonts/LeroyMerlinSans-Bold.woff2') format('woff2'),
        url('./assets/fonts/LeroyMerlinSans-Bold.woff') format('woff'),
        url('./assets/fonts/LeroyMerlinSans-Bold.ttf') format('truetype'),
        url('./assets/fonts/LeroyMerlinSans-Bold.svg#LeroyMerlinSans-Bold') format('svg');
    font-weight: bold;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: 'Leroy Merlin Sans';
    src: url('./assets/fonts/LeroyMerlinSans-Regular.eot');
    src: url('./assets/fonts/LeroyMerlinSans-Regular.eot?#iefix') format('embedded-opentype'),
        url('./assets/fonts/LeroyMerlinSans-Regular.woff2') format('woff2'),
        url('./assets/fonts/LeroyMerlinSans-Regular.woff') format('woff'),
        url('./assets/fonts/LeroyMerlinSans-Regular.ttf') format('truetype'),
        url('./assets/fonts/LeroyMerlinSans-Regular.svg#LeroyMerlinSans-Regular') format('svg');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}

#app { 
    display: grid; 
    grid-template-rows: 760px 50px;
    height: 100vh; 
    margin: 0;
    padding: 0;   
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
