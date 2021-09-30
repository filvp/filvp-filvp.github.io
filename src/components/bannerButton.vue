<template>
    <div><button class="bannerButton">
      Купить
    </button> </div>
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
.bannerButton {
    appearance: none;
    cursor: pointer;
    margin-top: 2em;
    margin-left: 3em;
    /* margin-bottom: 6em; */
    background-color: #00B21C;  
    border: 0; 
    line-height: 50px;
    color: white;   
    text-align: center;
    font-size: 45px; 
     font-family: 'Leroy Merlin Sans';
    font-weight: bold;    
    width: 10em;
    height: 3em;
    border-radius: 0.7em;
    -webkit-box-shadow: 0 0.4em 0 rgb(0 0 0 / 15%);
    box-shadow: 0 0.4em 0 rgb(0 0 0 / 15%);
}
@media screen and (max-width: 980px) { 
    .bannerButton {
        margin-left: 2em;
        margin-top: 1em;
        width: 7em;
        height: 2em;
        border-radius: 20px;
    }
}
</style>

