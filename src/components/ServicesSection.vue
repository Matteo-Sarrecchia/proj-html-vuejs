<script>
export default {
    name: "ServicesSection",
}
</script>

<template>
    <section class="services">
        <!-- col left -->
        <div class="col left">
            <!-- up -->
            <div class="slide up">
                <h3>
                    Graphic Design
                </h3>
                <div>
                    Have a passion for graphics and arts? Show your talents with confidence and self- assertiveness.
                </div>
                <img src="../../public/images/home-6-service-image-01.png" alt="">
            </div>

            <!-- down -->
            <div class="slide down">
                <img src="../../public/images/home-6-service-image-03.png" alt="">
                <h3>
                    Idea Discussion
                </h3>
                <div>
                    Get teamed up with the specialists who work and teach coding for years at famous universities.
                </div>
            </div>
        </div>

        <!-- col centre -->
        <div class="col centre">
            <!-- up -->
            <div class="slide up">
                <h3>
                    Business Administration</h3>
                <div>
                    Learners are encouraged to study the mechanism and structure of system administration.
                </div>
                <img src="../../public/images/home-6-service-image-02.png" alt="">
            </div>

            <!-- down -->
            <div class="slide down">
                <img src="../../public/images/home-6-service-image-04.png" alt="">
                <h3>
                    Web Development
                </h3>
                <div>
                    Learn to start building a webpage from scratch. You decide your own pace, course and speed.
                </div>
            </div>
        </div>

        <!-- col right -->
        <div class="col right">

            <div class="slide">
                <div>
                    TOGETHER WE CAN CREATE
                </div>
                <h2>
                    Services We <span>Can Provide</span> For My Clients.
                </h2>
                <ul>
                    <li>
                        <i class="fa-solid fa-check" style="color: #20ad96;"></i>
                        Select & customize courses to your preferences
                    </li>
                    <li>
                        <i class="fa-solid fa-check" style="color: #20ad96;"></i>
                        Change the tutor and make arrangements
                    </li>
                    <li>
                        <i class="fa-solid fa-check" style="color: #20ad96;"></i>
                        Participate in events to join others
                    </li>
                    <li>
                        <i class="fa-solid fa-check" style="color: #20ad96;"></i>
                        Get the desired certificate delivered at house
                    </li>
                </ul>
                <input type="button" value="Get started for free">
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

.services {
    min-height: 300px;
    width: 80%;
    margin: 0 auto;
    display: flex;
    padding: 50px 0;

    .left,
    .centre {
        width: 25%;

    }

    .left>div,
    .centre>div {
        min-height: 100px;
        margin: 10px;
    }

    .right {
        width: 50%;
        display: flex;
        align-items: center;
    }

    .slide {
        padding: 20px;
        background-color: #fff4f4;
        border-radius: 5px;

        h3 {
            margin-bottom: 10px;
        }

        img {
            margin-bottom: 10px;
        }
    }

    .col.centre .slide.up {
        margin-top: 80px;
    }

    .col.right .slide {
        width: 60%;
        min-height: 50%;

        h2 {
            font-size: 40px;
            padding: 20px 0;

            span {
                color: #20ad96;
            }
        }

        ul {
            list-style-type: none;

            li {
                margin: 10px 0;
            }
        }

        input {
            padding: 10px 30px;
            background-color: #20ad96;
            border: none;
            color: white;
            border-radius: 5px;

            &:hover {
                background-color: #3f3a64;
                color: white;
            }
        }
    }

}
</style>
