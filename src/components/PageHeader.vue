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
                    <li><a href="">Shop
                            <i class="fa-solid fa-chevron-down" style="color: #ffffff;"></i>
                            <i class="fa-regular fa-cart-shopping" style="color: #ffffff;"></i>
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
    border: 1px solid black;
    min-height: 100px;
    background: linear-gradient(180deg, #3f3a64 83%, #fff 17%);

    // menu navigazione
    nav {
        width: 70%;
        margin: 20px auto;
        height: 50px;
        display: flex;
        justify-content: space-between;

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
                }

                a {
                    color: white;
                    text-decoration: none;
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

            img {
                width: 100%;
                display: block;
            }

            #left,
            #right {
                width: 25%;
            }

            #left img {
                margin-left: 40px;
            }

            #right {
                background-image: url(../../public/images/home-6-hero-right-person-195x300.png);
                background-size: cover;
                margin-top: 115px;
            }

            #centre {
                width: 50%;
            }
        }

    }
}
</style>
