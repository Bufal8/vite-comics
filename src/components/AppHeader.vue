<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "Characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "Comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "Movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "Tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "Games",
                    url: "#",
                    current: false,
                },
                {
                    text: "Collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "Videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "Fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "News",
                    url: "#",
                    current: false,
                },
                {
                    text: "Shop",
                    url: "#",
                    current: false,
                },

            ]
        }
    }
}

</script>

<template>
    <header>
        <div class="container">
            <div class="logo">

                <a href="/" class="brand">
                    <img src="../assets/images/dc-logo.png" alt="dc">
                </a>

            </div>
            

            <nav>
                <ul>
                    <li v-for="link in links">
                        <a :href="link.url" :class="{ active :link.current }">{{ link.text }}</a>
                    </li>

                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header {
    // text-align: center;
    height: 100px;
    background-color: #ffffff;
    width: 100%;
    .container {
        display: flex;
        align-items: center;
        justify-content: space-around;
        align-items: center;
        height: 100%;
        width: 80%;

        .logo {
            width: 50%;
            height: 100%;
            @include center();
            justify-content: start;

            img{
                width: 60px;
                
            }
        }

        nav {
            height: 100%;
            width: 50%;

            ul {

                list-style-type: none;
                margin: 0;
                @include center();
                height: 100%;                
                
                li {
                    height: 100%;
                    width: 100%;
                    text-align: center;
                    margin-right: 10px;

                    &:active,
                    &:hover {

                        color: $primary;
                        border-bottom: 5px solid $primary;
                    }

                    a {
                        margin-top: 40px;
                        display: inline-block;
                        text-transform: uppercase;
                        text-decoration: none;
                        font-weight: 600;
                        font-size: 12px;
                        transition: background 0.3s;

                    }
                }
            }
        }
    }
}
</style>