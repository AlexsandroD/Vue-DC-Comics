<template>
  <main>
      <Jumbo/>
      <CardsProducts/>
  </main>
</template>

<script>
import Jumbo from"../sections/Jumbo.vue";
import CardsProducts from"../sections/CardsComics.vue";
export default {
name:'Main',
components:{
    Jumbo,
    CardsProducts,
},

}
</script>

<style scoped lang="scss">
@import "../../assets/styles/presets.scss";
main{
    background-color: black;
}
</style>