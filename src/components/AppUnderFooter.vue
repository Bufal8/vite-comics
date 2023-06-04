<script>
export default{
    name: "AppUnderFooter",
}
</script>

<template>
    <div class="container">

        <div class="sign-up">
            <a href="#">SIGN UP NOW!</a>
        </div>

        <div class="social">
            <h4>
                FOLLOW US
            </h4>

            <div class="social-links">
                <a href="#">
                    <img src="../assets/images/footer-facebook.png" alt="">
                </a>
                <a href="#">
                    <img src="../assets/images/footer-twitter.png" alt="">
                </a>
                <a href="#">
                    <img src="../assets/images/footer-youtube.png" alt="">
                </a>
                <a href="#">
                    <img src="../assets/images/footer-pinterest.png" alt="">
                </a>
                <a href="#">
                    <img src="../assets/images/footer-periscope.png" alt="">
                </a>
            </div>
        </div>

    </div>
</template>

<style lang="scss" scoped>

@use '../styles/partials/variables' as *;

@use '../styles/partials/mixins' as *;

.container{
    width: 80%;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .sign-up{
        border: 3px solid $primary;
        padding: 10px;

        a{
        color: #FFF;
        }
    }

    .social{
        display: flex;
        align-items: center;
        
        h4{
            margin-right: 15px;
            color: $primary;
        }

        a{
            width: 10px;
            margin-right: 10px;
        }
    }
}

</style>