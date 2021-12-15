<template>
  <footer id="footer">
        <div class="footer-top">
            <div class="container">
                <ul>
                    <li v-for="(link, index) in links" :key="index"><a href=""><img :src="link.src" :alt="link.alt"><span>{{link.text}}</span></a></li>
                  
                </ul>
            </div>
        </div>
        <div class="footer-middle">
                <div class="links">
                    <div class="comics-shop">
                        <ul>
                            <li class="white">Dc comics</li>
                            <li v-for="(dcComic,index) in dcComics.text" :key="index"><a href="dcComic.link">{{dcComic}}</a></li>
                        </ul>

                        <ul>
                            <li class="white">shop</li>
                            <li  v-for="(shop,index) in shops.text" :key="index"><a href="">{{shop}}</a></li>
                        </ul>
                    </div>
                    <ul>
                        <li class="white">DC</li>
                         <li  v-for="(dc,index) in dcs.text" :key="index"><a href="">{{dc}}</a></li>
                    </ul>
                    <ul>
                        <li class="white">Sites</li>
                         <li  v-for="(site,index) in sites.text" :key="index"><a href="">{{site}}</a></li>
                    </ul>

                
                   
                </div>
                <div class="dc-logo-big"><img src="../../assets/img/dc-logo-bg.png" alt="dc-logo-big"></div>
        </div>
      
            <div class="footer-bottom">
                <div class="container">
                    <div class="btn"><a href="">Sign-up now!</a></div>
                    <div class="links-icons">
                        <span>follow us</span>
                        <ul>
                            <li v-for="(icon, index) in icons" :key="index"><a :href="icon.href"><img :src="icon.srcIcona" alt="icon.alt"></a></li>
                        </ul>
                    </div>
                </div>
            </div>
      
  </footer>
</template>

<script>
export default {
data(){
    return{
        links:[
            {
                src:require("../../assets/img/buy-comics-digital-comics.png"),
                alt:"buy comics icon",
                text:'digital comics'
            },
            { 
                src:require("../../assets/img/buy-comics-merchandise.png"),
                alt:"buy comics icon",
                text:'digital comics'
            },
            {
                src:require("../../assets/img/buy-comics-subscriptions.png"),
                alt:"buy comics icon",
                text:'digital comics'
            },
            {
                src:require("../../assets/img/buy-comics-shop-locator.png"),
                alt:"buy comics icon",
                text:'digital comics'
            },
            {
                src:require("../../assets/img/buy-dc-power-visa.svg"),
                alt:"buy comics icon",
                text:'digital comics'
            }
        ],
        icons:[
            {   srcIcona:require("../../assets/img/footer-facebook.png"),
                href:"https://www.facebook.com/dc/",
                alt:'Icona social'
              
            },
            {
                srcIcona:require("../../assets/img/footer-twitter.png"),
                href:"https://twitter.com/dccomics",
                alt:'Icona social'

            },
            {
                srcIcona:require("../../assets/img/footer-youtube.png"),
                href:"https://www.youtube.com/channel/UCiifkYAs_bq1pt_zbNAzYGg",
                alt:'Icona social'

            },
            {
                srcIcona:require("../../assets/img/footer-pinterest.png"),
                href:"https://www.pinterest.co.uk/dccomics/",
                alt:'Icona social'
                
            },
            {
                srcIcona:require("../../assets/img/footer-periscope.png"),
                href:"https://www.twitter.com/dc/",
                alt:'Icona social'
            }
        ],
        dcComics:
            {
            text:["Characters","Comics","Movies","TV","Games","Videos","News"],
            link:'#'
            }
            ,
        shops:
            {
                text:["Shop DC","Shop DC Collectibles"],
            link:'#'
            }
        ,
        dcs:
            {
                text:["Terms of use","Privicy policy(New)","Ad Choises","Advertising","Jobs","Subscriptions","Talent Workshops","CPSC Certificates","Ratings","Shop Help","Contact Us"],
                link:'#'
            },
        sites:
            {text:["DC","MAD Magazine","DC kids","DC Universe","DC Power Visa"],
             link:'#'
            }
        

    }
}
}
</script>

<style scoped lang="scss">
@import '../../assets/styles/presets.scss';
    footer{
      display: flex;
      overflow: hidden;
      flex-direction: column;
      height: 37.5rem;
      width: 100%;
      background-image: url('../../assets/img/footer-bg.jpg');
      background-size: cover;

      .footer-top{
          position: relative;
          background-color: $main-color ;
          height: 6.25rem;
          ul{
              width: 100%;
              height: 100%;
              display: flex;
              justify-content: center;
              align-items: center;
              padding: 1.25rem;
              
              li{
                  display: flex;
                  align-items: center;
                  padding: 0.625rem 0.9375rem;
                      &:hover{
                          transform: scale(1.1);
                          transition: 0.2s;
                      }
                  a{
                      display: flex;
                      align-items: center;
                      img{
                          width: 2.5rem;
                          margin: 0rem 0.3125rem;
                      }
                  }
                  span{
                      text-transform: uppercase;
                      font-weight: 300;
                      color: white;
                  }
              }
          }
          z-index: 3;
      }
      .footer-middle{
          position: relative;
          width: 70%;
          margin: auto;
          display: flex;
          .links{
              display: flex;
              justify-content: space-between;
              width: 40%;
              height: 100%;
             ul{
                 margin: 0rem 0.625rem;
                  li{
                      padding:0.0625rem;
                      a{
                          color: rgba(255, 255, 255);
                          opacity: 0.6;
                          font-weight: lighter;
                          font-size: 0.75rem;
                          &:hover{
                              opacity: 1;
                          }
                      }
                  }
                
              }
          }
            
          .dc-logo-big{
              img{
                  position:absolute;
                  top: -30%;
                  left: 50%;
                  transform: translate(-50% -50%);
                  z-index: 1;
                  opacity: 0.8;
                  }
                    	
          }
      }
      .footer-bottom{
          display: flex;
          position: relative;
          height: 6.25rem;
          background-color: #303030;
          z-index: 2;
          .container{
              display: flex;
              justify-content: space-between;
              align-items: center;
              .btn{
                  outline: 0.125rem solid $main-color;
                  padding:0.5625rem 0;
                      &:hover{
                          outline-offset: 0.3125rem;
                      &:active{
                          transform: scale(0.98);
                      }
                      }
                  a{
                      color:white;
                      padding:1.25rem;
                      text-transform: uppercase;
                  }
              }
              .links-icons{
                  display: flex;
                  align-items: center;
                  span{
                      color: $main-color;
                      text-transform: uppercase;
                      font-weight: bold;
                      padding: 0.3125rem;
                  }
                  ul{
                      display: flex;
                      li{
                          padding:0.625rem;
                          &:hover{
                              opacity: 0.7;
                          }
                      }
                  }
              }
          }
      }

    }
</style>