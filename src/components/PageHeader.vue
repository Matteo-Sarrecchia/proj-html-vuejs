<script>
export default {
    name: "PageHeader"
}
</script>

<template>
    <!-- header -->
    <header>
        <!-- menu navigazione -->
        <nav>
            <div id="logo">
                <img src="../../public/images/light-logo.png" alt="logo max coach">
            </div>
            <div id="menu-nav">
                <ul>
                    <li><a href="">Home
                            <i class="fa-solid fa-chevron-down" style="color: #ffffff;"></i>
                        </a></li>
                    <li>
                        <a href="">Pages
                            <i class="fa-solid fa-chevron-down" style="color: #ffffff;"></i>
                        </a>
                    </li>
                    <li><a href="">Courses
                            <i class="fa-solid fa-chevron-down" style="color: #ffffff;"></i>
                        </a>
                    </li>
                    <li><a href="">Features
                            <i class="fa-solid fa-chevron-down" style="color: #ffffff;"></i>
                        </a>
                    </li>
                    <li><a href="">Blog
                            <i class="fa-solid fa-chevron-down" style="color: #ffffff;"></i>
                        </a>
                    </li>
                    <li>
                        <a href="">Shop
                            <i class="fa-solid fa-chevron-down" style="color: #ffffff;"></i>
                            <i class="fa-solid fa-cart-shopping shop" style="color: #ffffff;"></i>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <i class="fa-solid fa-circle-user" style="color: #ffffff;"></i>
                        </a>
                    </li>
                    <li>
                        <div id="search">
                            <input type="text" value="" placeholder="Search">
                            <i class="fa-solid fa-magnifying-glass" style="color: blue;"></i>
                        </div>
                    </li>
                </ul>
            </div>
        </nav>

        <!-- jumbotron -->
        <div class="jumbotron">
            <h1>Learn At Your Own Pace!</h1>
            <h3>Get teamed up with people of the same will.</h3>
            <div>
                <input type="button" value="Get started for free">
            </div>
            <div class="container">
                <div id="left">
                    <img src="/images/home-6-hero-left-person.png" alt="">
                </div>
                <div id="centre">
                    <img src="/images/home-6-hero-poster-final.jpg" alt="">
                    <img id="img-youtube" src="../../public/images/icon-youtube-play.png" alt="">
                </div>
                <div id="right">

                </div>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

header {
    min-height: 100px;
    background-color: #303060;
    background-image: url(../../public/images/header-background.png);
    // background: linear-gradient(180deg, #3f3a64 83%, #fff 17%);

    // menu navigazione
    nav {
        width: 70%;
        margin: 0 auto;
        height: 50px;
        display: flex;
        justify-content: space-between;
        padding-top: 30px;

        #logo {
            width: 20%;

            img {
                width: 100%;
            }
        }

        #menu-nav {
            width: 65%;
            display: flex;
            align-items: center;

            ul {
                list-style-type: none;
                display: flex;
                width: 100%;
                justify-content: space-between;

                li {
                    display: flex;
                    align-items: center;

                    &:hover {
                        border-bottom: 1px solid white;
                    }
                }

                a {
                    color: white;
                    text-decoration: none;

                    .shop {
                        margin-left: 5px;
                    }
                }

                #search {
                    background-color: white;

                    input {
                        padding: 10px;
                        border: none;
                    }

                    i {
                        margin: 10px;
                    }
                }
            }
        }
    }

    // jumbotron
    .jumbotron {
        width: 80%;
        margin: 50px auto;
        min-height: 100px;
        color: white;
        text-align: center;

        h1,
        h3,
        input {
            margin-bottom: 30px;
        }

        h3 {
            color: rgba($color: #ffffff, $alpha: 0.6)
        }

        input {
            background-color: #20ad96;
            padding: 10px 30px;
            color: white;
            border: none;
            border-radius: 5px;

            &:hover {
                background-color: white;
                color: lightskyblue;
            }
        }

        .container {
            min-height: 100px;
            display: flex;
            margin-bottom: -110px;

            img {
                width: 100%;
                display: block;
            }

            #left {
                width: 25%;
            }

            #right {
                width: 20%;
                background-image: url(../../public/images/home-6-hero-right-person-195x300.png);
                background-size: cover;
                margin-top: 170px;
            }

            #left img {
                margin-left: 40px;
            }


            #centre {
                width: 50%;
                position: relative;

                #img-youtube {
                    width: 80px;
                    position: absolute;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                }
            }
        }

    }
}
</style>
