<script>
export default {
    name: "PageFooter"
}
</script>

<template>
    <footer>
        <div class="container">

            <!-- col left -->
            <div class="col left">
                <ul>
                    <li>
                        <h3>Address</h3>
                    </li>
                    <li>
                        <a href="">382 NE 191st St # 87394 Miami, FL 33179-3899</a>
                    </li>
                    <li>
                        <a href="">+1 (305) 547-9909 (9am - 5pm EST, Monday - Friday)</a>
                    </li>
                    <li>
                        <a href="">support@maxcoach.com</a>
                    </li>
                    <li>
                        <a href="" class="social">
                            <i class="fa-brands fa-square-facebook" style="color: #8c8c8c;"></i>
                        </a>
                        <a href="" class="social">
                            <i class="fa-brands fa-twitter" style="color: #8c8c8c;"></i>
                        </a>
                        <a href="" class="social">
                            <i class="fa-brands fa-square-instagram" style="color: #8c8c8c;"></i>
                        </a>
                        <a href="" class="social">
                            <i class="fa-brands fa-linkedin" style="color: #8c8c8c;"></i>
                        </a>
                    </li>
                </ul>
            </div>

            <!-- col centre -->
            <div class="col centre">
                <ul>
                    <li>
                        <h3>Explore</h3>
                    </li>
                    <li>
                        <span>
                            <a href="">Start here</a>
                        </span>
                        <a href="">Success story</a>
                    </li>
                    <li>
                        <span>
                            <a href="">Blog</a>
                        </span>
                        <a href="">Courses</a>
                    </li>
                    <li>
                        <span>
                            <a href="">About us</a>
                        </span>
                        <a href="">Contact us</a>
                    </li>
                </ul>
            </div>

            <!-- col right -->
            <div class="col right">
                <ul>
                    <li>
                        <h3>Information</h3>
                    </li>
                    <li>
                        <a href="">Membership</a>
                    </li>
                    <li>
                        <a href="">Purchase guide</a>
                    </li>
                    <li>
                        <a href="">Privacy policy</a>
                    </li>
                    <li>
                        <a href="">Terms of services</a>
                    </li>
                </ul>
            </div>
        </div>
        <div id="footer-text">
            © 2020 Maxcoach. All Rights Reserved
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

footer {
    min-height: 100px;

    .container {
        width: 70%;
        margin: 50px auto;
        min-height: 100px;
        display: flex;

        .col {
            min-height: 50px;

            ul {
                list-style-type: none;

                li {
                    margin-bottom: 20px;

                    a {
                        text-decoration: none;
                        color: rgba($color: #000000, $alpha: 0.6);

                        &:hover {
                            text-decoration: underline;
                            color: blue;
                        }


                    }
                }
            }
        }

        .left {
            width: 50%;

            .social {
                margin-right: 20px;
                font-size: 30px;
            }
        }

        .centre {
            width: 25%;

            span {
                width: 40%;
                display: inline-block;
            }
        }

        .right {
            width: 25%;
        }
    }

    #footer-text {
        text-align: center;
        margin-bottom: 50px;
        color: rgba($color: #000000, $alpha: 0.6);
    }
}
</style>
