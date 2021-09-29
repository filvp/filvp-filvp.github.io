<template>
     <div class="videoBlock">
                <video width="405" height="230" controls="controls" poster="../assets/i/video.png">
                  <source src="../assets/i/video.mp4" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'>                  
                </video>   
       <div class="bannerMute">       
        <!-- <img src="../assets/i/close.svg"> -->
        <img src="../assets/i/mute.svg">
       </div>           
    </div>
</template>

<script>
export default {
  data() {
    return {
      dynamicComponent: null
    }
  },
}
</script>
<style scoped>
.videoBlock {
  width: 600px; 
  margin-top: 4em; 
  margin-left: 4em;
  display: flex;
  justify-content: space-between;
 
   
    /* height: 50vh !important;
    width: 50vw;
    left: 50vw;
    top: 0; */
}
.bannerMute img{
  width: 60px;  
  margin-top: 2em;
}

@media screen and (max-width: 980px) {
    .videoBlock {
    width: 370px;
    }
}

@media (orientation: landscape) {
    /* .video-wrapper {
      margin: 0 auto;
}     */
}
</style>