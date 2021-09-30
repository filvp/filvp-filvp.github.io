<template>
     <div class="footer">
        <p class="footerText">Leroymerlin.ru</p>     
            <div class="bannerLogo">
        <img src="../assets/i/logo.jpg">      
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
.footer {
    display: flex;
    align-items: center;
    align-content: flex-end;
    justify-content: space-between;
    background-color: #00B21C;
    width: 100%;
    color: white;   
    text-align: center;
    font-size: 22px;         
    position: absolute;
    /* font-size: 0.8em; */
    line-height: 100%;
    font-weight: 900;
    text-align: center;
    font-family: 'Leroy Merlin Sans';
    font-weight: normal;
    height: 50px;
    bottom: 0;
    overflow: hidden;   
}
.bannerLogo{
  /* display: flex; */
  height: 70px;
  box-shadow: 2 0.4 0 black;
  margin-right: 0.7em; 
  bottom: 0;
}
.footerText {
  margin-left: 50%;
}

@media screen and (max-width: 980px) {
  
.footer {
    position: relative;
    margin-top: 7em;   
}
.footerText {
  margin-left: 30%;
}
}
</style>
 
 
 