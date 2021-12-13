<template>
  <footer>
        <div class="footer-top">
            <div class="container">
                <ul>
                    <li><a href=""><img src="../assets/img/buy-comics-digital-comics.png" alt="buy comics icon"></a><span>digital comics</span></li>
                    <li><a href=""><img src="../assets/img/buy-comics-merchandise.png" alt="buy merchandise icon"></a><span>digital comics</span></li>
                    <li><a href=""><img src="../assets/img/buy-comics-subscriptions.png" alt="buy subscriptions icon"></a><span>digital comics</span></li>
                    <li><a href=""><img src="../assets/img/buy-comics-shop-locator.png" alt="shop-locator icon"></a><span>digital comics</span></li>
                    <li><a href=""><img src="../assets/img/buy-dc-power-visa.svg" alt="power-visa icon"></a><span>digital comics</span></li>
                </ul>
            </div>
        </div>
        <div class="footer-middle">
                <div class="links">
                    <div class="comics-shop">
                        <ul>
                            <li class="white">Dc comics</li>
                            <li><a href="">links</a></li>
                            <li><a href="">links</a></li>
                            <li><a href="">links</a></li>
                            <li><a href="">links</a></li>
                            <li><a href="">links</a></li>
                            <li><a href="">links</a></li>
                            <li><a href="">links</a></li>
                        </ul>

                        <ul>
                            <li class="white">shop</li>
                            <li><a href="">links</a></li>
                            <li><a href="">links</a></li>  
                        </ul>
                    </div>
                    <ul>
                        <li class="white">Dc comics</li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                    </ul>
                    <ul>
                        <li class="white">Dc comics</li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                        <li><a href="">links</a></li>
                    </ul>

                
                   
                </div>
                <div class="dc-logo-big"><img src="../assets/img/dc-logo-bg.png" alt="dc-logo-big"></div>
        </div>
      
            <div class="footer-bottom">
                <div class="container">
                    <div class="btn"><a href="">Sign-up now!</a></div>
                    <div class="links-icons">
                        <span>follow us</span>
                        <ul>
                            <li><a href=""><img src="../assets/img/footer-facebook.png" alt=""></a></li>
                            <li><a href=""><img src="../assets/img/footer-twitter.png" alt=""></a></li>
                            <li><a href=""><img src="../assets/img/footer-youtube.png" alt=""></a></li>
                            <li><a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a></li>
                            <li><a href=""><img src="../assets/img/footer-periscope.png" alt=""></a></li>
                        </ul>
                    </div>
                </div>
            </div>
      
  </footer>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
@import '../assets/styles/presets.scss';
    footer{
      display: flex;
      overflow: hidden;
      flex-direction: column;
      height: 600px;
      width: 100%;
      background-image: url('../assets/img/footer-bg.jpg');
      background-size: cover;

      .footer-top{
          position: relative;
          background-color: $main-color ;
          height: 100px;
          ul{
              width: 100%;
              height: 100%;
              display: flex;
              justify-content: center;
              align-items: center;
              padding: 20px;
              
              li{
                  display: flex;
                  align-items: center;
                  padding: 10px 15px;
                  a{
                      &:hover{
                          transform: scale(1.1);
                      }
                      img{
                          width: 40px;
                          margin: 0px 5px;
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
              width: 30%;
              height: 100%;
             ul{
                  li{
                      padding:5px;
                      a{
                          color: rgba(255, 255, 255);
                          opacity: 0.6;
                          font-weight: lighter;
                          font-size: 12px;
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
          height: 100px;
          background-color: #303030;
          z-index: 2;
          .container{
              display: flex;
              justify-content: space-between;
              align-items: center;
              .btn{
                  outline: 2px solid $main-color;
                  padding:9px 0;
                      &:hover{
                          outline-offset: 5px;
                      &:active{
                          transform: scale(0.98);
                      }
                      }
                  a{
                      color:white;
                      padding:20px;
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
                      padding: 5px;
                  }
                  ul{
                      display: flex;
                      li{
                          padding:10px;
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