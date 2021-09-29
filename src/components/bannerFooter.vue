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
    background-color: green;
    width: 100%;
    color: white;   
    text-align: center;
    font-size: 18px;         
    position: absolute;
    font-size: 0.8em;
    line-height: 120%;
    font-weight: 900;
    text-align: center;
    font-family: 'LeroyMerlinSans', Arial, Helvetica, sans-serif;
    font-weight: normal;
}
.bannerLogo{
  display: flex;
  height: 60px;
}
.footerText {
  margin-left: 50%;
}
</style>
 
 
 