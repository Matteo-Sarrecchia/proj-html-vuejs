<script>
export default {
    name: "TalkAboutSection"
}
</script>

<template>
    <section class="talkAbout" style="margin: auto; padding: 50px 0;">
        <h1>
            Why People Talk About <span>MaxCoach</span> ?
        </h1>
        <div class="container">
            <div class="card">
                <img src="../../public/images/testimonial-avata-02.jpg" alt="">
            </div>
            <div class="text">
                <div id="main-text">
                    I am free to learn at my own pace, follow my own schedule and choose the subject | like. Great study
                    portal for people like me.
                </div>
                <div id="name">MINA HOLLACE</div>
                <div>/Freelancer</div>
            </div>
        </div>
        <div class="sponsor">
            <div class="col">
                <a href="">
                    <img src="../../public/images/client-logo-colored-01.png" alt="">
                </a>
            </div>
            <div class="col">
                <a href="">
                    <img src="../../public/images/client-logo-colored-02.png" alt="">
                </a>
            </div>
            <div class="col">
                <a href="">
                    <img src="../../public/images/client-logo-colored-03.png" alt="">
                </a>
            </div>
            <div class="col">
                <a href="">
                    <img src="../../public/images/client-logo-colored-04.png" alt="">
                </a>
            </div>
            <div class="col">
                <a href="">
                    <img src="../../public/images/client-logo-colored-05.png" alt="">
                </a>
            </div>
            <div class="col">
                <a href="">
                    <img src="../../public/images/client-logo-colored-06.png" alt="">
                </a>
            </div>

        </div>
    </section>
</template>

<style lang="scss">
@use "../styles/generals.scss" as *;

.talkAbout {
    min-height: 50px;
    width: 80%;
    text-align: center;
    padding: 50px 0;

    h1 {
        font-size: 50px;
        margin: 20px 0;

        span {
            color: #20ad96;
            font-weight: initial;
        }
    }

    .container {
        display: flex;
        justify-content: center;

        .card {
            width: 200px;
            height: 200px;
            background-image: url(../../public/images/maxcoach-shape-05-100x100.png);
            background-size: 50%;
            background-repeat: no-repeat;
            background-position-x: right;
            background-position-y: bottom;

            img {
                width: 100%;
                height: 100%;
                border-radius: 50%;
                padding: 10px;
            }
        }

        .text {
            width: 60%;
            text-align: left;
            margin-left: 30px;

            #name {
                font-weight: bold;
            }

            #main-text {
                font-size: 30px;
            }

            div {
                padding: 10px 20px;
            }
        }
    }

    .sponsor {
        margin: 30px 0;
        min-height: 50px;
        display: flex;

        .col {
            width: calc(100% / 6);
            min-height: 50px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
    }

}
</style>
