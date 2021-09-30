<template>
     <div class="videoBlock">
                <video autoplay="autoplay" width="570" height="320" muted="muted" controls="controls" poster="../assets/i/video.png">
                  <source src="../assets/i/video.mp4" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"'>                  
                </video>   
       <div class="bannerMute">       
        <div><img src="../assets/i/close.svg"></div>
        <div class='mute'><img src="../assets/i/mute.svg"></div>
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
  width: 700px; 
  margin-top: 2em; 
  margin-left: 6em;
  display: flex;
  justify-content: space-between;
 
   
    /* height: 50vh !important;
    width: 50vw;
    left: 50vw;
    top: 0; */
}

.bannerMute img{
  width: 70px;  
  /* margin-top: 2em; */
}
.bannerMute{
  display: flex;
  flex-direction: column; 
}

.mute{
  margin-top: 10em;
}

@media screen and (max-width: 980px) {
    .videoBlock {
    width: 430px;
    }
    .mute{
    margin-top: 7em;
}
video{
  width: 420px;
  height: 230px;
}

.bannerMute img{
  width: 50px;  
  margin-left: .5em;
  /* margin-top: 2em; */
}
}

@media (orientation: landscape) {
    /* .video-wrapper {
      margin: 0 auto;
}     */
}
</style>