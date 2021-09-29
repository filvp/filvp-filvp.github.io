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
    margin-left: 2em;
    margin-bottom: 6em;
    background-color: green;  
    border: 0; 
    line-height: 50px;
    color: white;   
    text-align: center;
    font-size: 28px; 
    font-family: 'LeroyMerlinSans-Regular';     
    width: 9em;
    height: 2.5em;
    border-radius: 0.4em;
    -webkit-box-shadow: 0 0.4em 0 rgb(0 0 0 / 15%);
    box-shadow: 0 0.4em 0 rgb(0 0 0 / 15%);
}
@media screen and (max-width: 980px) { 
    .bannerButton {
        margin-left: 4.5em;
        margin-top: 2em;
    }
}
</style>