
export default {
<script>
export default{
    name: "AppBanner",
}

</script>

<template>
  
    <main>
      
      <div class="container">
        
        <div class="item">
          
          <div class="img-item">

            <img src="../assets/images/buy-comics-digital-comics.png" alt="">

          </div>

          <div class="txt-item">
          
            <h6>DIGITAL COMICS</h6>

          </div>

        </div>
        
        <div class="item">
        
          <div class="img-item">

            <img src="../assets/images/buy-comics-merchandise.png" alt="">

          </div>

          <div class="txt-item">          

            <h6>DC MERCHANDISE</h6>

          </div>

        </div>
        
        <div class="item">
          
          <div class="img-item">          

            <img src="../assets/images/buy-comics-shop-locator.png" alt="">

          </div>

          <div class="txt-item">          

            <h6>SUBSCRIPTION</h6>

          </div>

        </div>
        
        <div class="item">
          

          <div class="img-item">          

            <img src="../assets/images/buy-comics-subscriptions.png" alt="">

          </div>          

          <div class="txt-item">          

            <h6>COMIC SHOP LOCATOR</h6>

          </div>

        </div>
        
        <div class="item">
          
          <div class="img-item">          

            <img style="width: 50px; margin-right: 20px; margin-top: 8px;" src="../assets/images/buy-dc-power-visa.svg" alt="">

          </div>

          <div class="txt-item">          

            <h6>DC POWER VISA</h6>

          </div>

        </div>

      </div>
    
    </main>

</template>

<style lang="scss" scoped>

    @use '../styles/partials/variables' as *;

    @use '../styles/partials/mixins' as *;

    main {
      background-color: $primary;
      padding: 50px 0;
      .container {
        width: 80%;
        @include center();
        justify-content: space-between; 

        .item {
          display: flex;
          align-items: center;
          width: 15%;

          .img-item{
            width: 50px;
            height: 50px;

            img{
              max-width: 50px;
              max-height: 50px;
            }

          }

          .txt-item{
            font-size: 16px;
          }

        }
      }
    }
</style>