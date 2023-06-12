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
            
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

header {
    border: 1px solid black;
    min-height: 100px;
    background-color: blue;

    // menu navigazione
    nav {
        width: 80%;
        margin: 10px auto;
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
            width: 60%;
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
                        margin-right: 10px;
                    }
                }
            }
        }
    }

    // jumbotron
    .jumbotron {
        width: 80%;
        margin: 0 auto;
        border: 1px solid black;
        min-height: 100px;
    }
}
</style>
