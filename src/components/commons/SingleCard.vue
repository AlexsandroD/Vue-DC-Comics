<template>
        <div class="card">
            <img :src="card.thumb" :alt="card.type">
            <div class="title">{{card.series}}</div>
        </div>
</template>

<script>
export default {
    name:'SingleCard',
    props: {
        card: Object
    }
}
</script>

<style lang="scss" scoped>
     .card{
            width:15%; 
            .title{
                color: white;
                padding:5px 0;
            }
            img{
                width: 100%;
                aspect-ratio: 1 / 1;
                object-fit: cover;
                object-position: 0px 10px; 
            }

            &:hover{
             transform: scale(1.2);
                }
         
        }
</style>