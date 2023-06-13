<script>
export default {
    name: "HelpYouSection",
}

</script>

<template>
    <section class="help">
        <h3>
            WANNA TRANSFORM YOUR LIFE?
        </h3>
        <h1>
            Glad to <span>Help You</span> Learn
        </h1>
        <div class="container">
            <!-- col 1 -->
            <div class="col">
                <div class="icons">
                    <i class="fa-regular fa-flag" style="color: #6b6b6b;"></i>
                </div>
                <h4>Idea Discussion</h4>
                <div class="text">
                    Get teamed up with the specialists who work and teach coding for years at famous universities.
                </div>
            </div>

            <!-- col 2 -->
            <div class="col">
                <div class="icons">
                    <i class="fa-solid fa-gear" style="color: #6b6b6b;"></i>
                </div>
                <h4>Web Development</h4>
                <div class="text">
                    Learn to start building a webpage from scratch. You decide your own pace, course and speed.
                </div>
            </div>

            <!-- col 3 -->
            <div class="col">
                <div class="icons">
                    <i class="fa-regular fa-life-ring" style="color: #6b6b6b;"></i>
                </div>
                <h4>System Administration</h4>
                <div class="text">
                    Learners are encouraged to study the mechanism and structure of system administration.
                </div>
            </div>

            <!-- col 4 -->
            <div class="col">
                <div class="icons">
                    <i class="fa-solid fa-desktop" style="color: #6b6b6b;"></i>
                </div>
                <h4>Graphic Designn</h4>
                <div class="text">
                    Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.
                </div>
            </div>
        </div>
        <div class="img">
            <img src="../../public/images/home-6-services-image.png" alt="">
        </div>
        <div id="title-sub">Start today for getting <span>Online Certification</span>
            <h2>You can be your own guiding star with our help!</h2>
            <input type="button" value="Get started now">
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

.help {
    min-height: 100px;
    padding: 50px 0;
    background: rgb(182, 179, 179);
    background: linear-gradient(0deg, rgba(182, 179, 179, 1) 0%, rgba(255, 255, 255, 1) 80%);

    h3 {
        font-size: 20px;
        margin: 20px 0;
        color: rgba($color: #000000, $alpha: 0.6);
        text-align: center;
    }

    h1 {
        text-align: center;
        font-size: 50px;
        margin: 20px 0;

        span {
            color: #20ad96;
            font-weight: initial;
        }
    }

    .container {
        width: 80%;
        margin: 50px auto;
        display: flex;


        .col {
            width: calc(100% / 4 - 40px);
            margin: 20px;
            min-height: 100px;

            .icons {
                font-size: 50px;
            }

            h4,
            .text {
                margin-top: 10px;
            }

            .text {
                color: rgba($color: #000000, $alpha: 0.6);
            }
        }

    }

    .img {
        text-align: center;
        padding-bottom: 40px;
    }

    #title-sub {
        font-size: 24px;
        text-align: center;
        font-weight: bold;

        span {
            color: #20ad96;
            font-weight: initial;
        }

        input {
            padding: 10px 30px;
            background-color: #20ad96;
            border: none;
            color: white;
            border-radius: 5px;
            margin: 20px 0;

            &:hover {
                background-color: #3f3a64;
                color: white;
            }
        }
    }
}
</style>
