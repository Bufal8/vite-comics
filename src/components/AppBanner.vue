
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
          
            <h5>DIGITAL COMICS</h5>

          </div>

        </div>
        
        <div class="item">
        
          <div class="img-item">

            <img src="../assets/images/buy-comics-merchandise.png" alt="">

          </div>

          <div class="txt-item">          

            <h5>DC MERCHANDISE</h5>

          </div>

        </div>
        
        <div class="item">
          
          <div class="img-item">          

            <img src="../assets/images/buy-comics-shop-locator.png" alt="">

          </div>

          <div class="txt-item">          

            <h5>SUBSCRIPTION</h5>

          </div>

        </div>
        
        <div class="item">
          

          <div class="img-item">          

            <img src="../assets/images/buy-comics-subscriptions.png" alt="">

          </div>          

          <div class="txt-item">          

            <h5>COMIC SHOP LOCATOR</h5>

          </div>

        </div>
        
        <div class="item">
          
          <div class="img-item">          

            <img style="width: 60px; margin-right: 20px;" src="../assets/images/buy-dc-power-visa.svg" alt="">

          </div>

          <div class="txt-item">          

            <h5>DC POWER VISA</h5>

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
    display: flex;
    align-items: center;
    justify-content: space-between;  

    .item {
      display: flex;
      align-items: center;

      img{
        width: 50%;
        }

      }
    }
}
</style>