<template>
  <header>
      <div class="container">
      <div class="logo"><img src="../../assets/img/dc-logo.png" alt="Logo Dc"></div>
      <div class="nav">
          <ul>
              <li v-for="(nav,index) in navs" :key="index"><a :href="nav.href">{{nav.navLi}}</a></li>
          </ul>
      </div>
      </div>
  </header>
</template>

<script>
export default {
name:"Header",
data(){
  return{
      navs:[
          {
              navLi:'characters',
              href:'#footer',
              state:false
          },
          {
              navLi:'comics',
              href:'#',
              state:false
          },
          {
              navLi:'movies',
              href:'#',
              state:false
          },
          {
              navLi:'tv',
              href:'#',
              state:false
          },
          {
              navLi:'games',
              href:'#',
              state:false
          },
          {
              navLi:'collectibles',
              href:'#',
              state:false
          },
          {
              navLi:'videos',
              href:'#',
              state:false
          },
          {
              navLi:'fans',
              href:'#',
              state:false
          },
          {
              navLi:'news',
              href:'#',
              state:false
          },
          {
              navLi:'shop',
              href:'#',
              state:false
          },
      ]
  }
}
}
</script>

<style scoped lang="scss">
@import "../../assets/styles/presets.scss";
    header{
        height: 100px;

       
     .logo{
            display: flex;
            align-items: center;
            justify-content: start;
            width: 20%;
            height: 100%;
            margin-right: 100px;
            img{
                width: 60px;
            }
        }
     .nav{
         display: flex;
         justify-content: center;
         align-items: center;
         height: 100%;
         width: 80%;
         ul{
             display: flex;
             height: 100%;
             align-items: center;
                
                     }
             li{
                 display: flex;
                 align-items: center;
                 height: 100%;
                 list-style: none;
                 padding: 0px 10px;
                 text-transform: uppercase;

                 &:hover {
                     border-bottom: 5px solid $main-color ;
                     transition: 0.2s;

                 }

                 a{
                     display: flex;
                     align-items: center;
                     height: 100%;
                     text-decoration: none;
                     color: black;
                     font-weight: 600;
                     &:hover{
                        color:$main-color;
                        transition: 0.2s;
                        }
               
             }
         }
     }
    }
</style>