<template>
  <div class="jumbo">
       <label for="">current series</label>
  </div>
</template>

<script>
export default {
name:'Jumbo'
}
</script>

<style scoped lang="scss">
@import "../../assets/styles/presets.scss";

    .jumbo{
        position: relative;
        background-image: url("../../assets/img/jumbotron.jpg");
        height: 350px;
        background-size: cover;
        background-repeat: no-repeat;
        
     label{
        position: absolute;
        bottom: -20px;
        left: 200px;
        background-color: $main-color;
        font-size: 20px;
        padding: 10px 20px;
        color: white;
        text-transform: uppercase;
        font-weight: bold;

    }
    }
</style>