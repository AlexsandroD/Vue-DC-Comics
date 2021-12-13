<template>
  <footer>
        <div class="footer-top">
            <ul>
                <li><a href=""><img src="../assets/img/buy-comics-digital-comics.png" alt="buy comics icon"></a><span>digital comics</span></li>
                <li><a href=""><img src="../assets/img/buy-comics-merchandise.png" alt="buy merchandise icon"></a><span>digital comics</span></li>
                <li><a href=""><img src="../assets/img/buy-comics-subscriptions.png" alt="buy subscriptions icon"></a><span>digital comics</span></li>
                <li><a href=""><img src="../assets/img/buy-comics-shop-locator.png" alt="shop-locator icon"></a><span>digital comics</span></li>
                <li><a href=""><img src="../assets/img/buy-dc-power-visa.svg" alt="power-visa icon"></a><span>digital comics</span></li>
            </ul>
        </div>
        <div class="footer-middle"></div>
        <div class="footer-bottom"></div>
     
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
      flex-direction: column;
      height: 500px;
      width: 100%;
      background-image: url('../assets/img/footer-bg.jpg');
      background-size: cover;
      .footer-top{
          background-color: $main-color ;
          height: 100px;
          ul{
              width: 100%;
              height: 100%;
              display: flex;
              justify-content: center;
              align-items: center;
              
              li{
                  display: flex;
                  align-items: center;
                  padding: 20px;
                  a{
                      img{
                          width: 50px;
                          margin: 0px 10px;
                      }
                  }
                  span{
                      text-transform: uppercase;
                      font-weight: 300;
                      color: white;
                  }
              }
          }
      }
      .footer-middle{
          height: calc(100% - 200px);
      }
      .footer-bottom{
          height: 100px;
          background-color: black;
      }

    }
</style>