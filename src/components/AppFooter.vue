<script>
export default {
    name: "AppFooter",
    methods: {
        getImageURL: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }
}

</script>

<template>
    <footer>
        <div class="cols container">
            

            <div class="footer-links">
                <h4>DC COMICS</h4>

                <nav>
                    <ul>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Video</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                </nav>

                <h4>SHOP</h4>
                <nav>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </nav>
            </div>
            <div class="footer-links">
                <h4>DC</h4>

                <nav>
                    <ul>
                        <li><a href="#">Terms Of Use</a></li>
                        <li><a href="#">Privacy policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">Talent Workshops</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </nav>

            </div>

            <div class="footer-links">
                <h4>SITES</h4>
                <nav>
                    <ul>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Universe</a></li>
                        <li><a href="#">DC Power Visa</a></li>
                    </ul>
                </nav>
            </div>

            <a class="logo" href="/">
                <img src="../assets/images/dc-logo-bg.png" alt="dc">
            </a>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

footer {
    background-image: url("../assets/images/footer-bg.jpg");

    .container{
        width: 80%;
        height: 100%;

    }
    .cols {

        display: flex;
        justify-content: space-between;
        // margin-bottom: 3rem;

        .logo{

            img{
                height: 100%;
                width: auto;
            }
        }
        .footer-links {
            margin: 3rem 0;
            flex-basis: calc(100% / 6);
            text-align: start;
        }

        h4 {
            text-transform: uppercase;
            font-size: 1.25rem;
            font-weight: 600;
            margin-bottom: 1rem;
        }

        ul {
            list-style: none;

            li a {

                display: inline-block;
                margin-bottom: 0.25rem;
                text-decoration: none;
                font-size: 0.875em;
                color: #797979;

                &:hover,
                &:active {
                    color: $primary;
                }
            }
        }
    }
}
</style>