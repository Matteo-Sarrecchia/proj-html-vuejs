<script>

export default {
    name: "CoursesSection",
    data() {
        return {
            listCorsi: [
                {
                    id: 1,
                    price: "$40.00",
                    text: "Learning to Write as a Professional Author",
                    nLessons: "20 Lessons",
                    nStudents: "50 Students",
                    img: "../../public/images/course-02-480x298.jpg"
                },
                {
                    id: 2,
                    price: "Free",
                    text: "Customer-centric Info-Tech Strategies",
                    nLessons: "24 Lessons",
                    nStudents: "769 Students",
                    img: "../../public/images/stock-full-hd-03-480x298.jpg"
                },
                {
                    id: 3,
                    price: "$19.00",
                    text: "Open Programming Courses for Everyone: Python",
                    nLessons: "17 Lessons",
                    nStudents: "62 Students",
                    img: "../../public/images/stock-full-hd-04-480x298.jpg"
                },
                {
                    id: 4,
                    price: "$26.00",
                    text: "Academic Listening and Note- taking",
                    nLessons: "14 Lessons",
                    nStudents: "67 Students",
                    img: "../../public/images/stock-full-hd-06-480x298.jpg"
                },
                {
                    id: 5,
                    price: "$39.00",
                    text: "Master jQuery in a Short Period of Time",
                    nLessons: "6 Lessons",
                    nStudents: "51 Students",
                    img: "../../public/images/course-featured-image-01-480x298.jpg"
                },
                {
                    id: 6,
                    price: "$59.00",
                    text: "Introduction to Javascript for Beginners",
                    nLessons: "14 Lessons",
                    nStudents: "76 Students",
                    img: "../../public/images/stock-full-hd-05-480x298.jpg"
                },
            ]
        }
    }
}
</script>

<template>
    <section class="course">
        <h3>
            CHOOSE A COURSE TO GET STARTED
        </h3>
        <h1>
            Latest Featured <span>Courses</span>
        </h1>
        <div class="container">

            <div class="card" v-for="elm in listCorsi">
                <div class="card-img">
                    <img :src="elm.img" alt="">
                </div>
                <div class="card-text">
                    <div class="price">
                        {{ elm.price }}
                    </div>
                    <div class="text">
                        {{ elm.text }}
                    </div>
                    <div>
                        <span>
                            <i class="fa-solid fa-file-lines" style="color: #ffffff;"></i>
                            {{ elm.nLessons }}
                        </span>
                        <span>
                            <i class="fa-regular fa-user" style="color: #ffffff;"></i>
                            {{ elm.nStudents }}
                        </span>
                    </div>
                </div>
            </div>
        </div>
        <input type="button" value="View all courses  →">
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

.course {
    min-height: 300px;
    margin: 0 auto;
    text-align: center;
    padding: 50px 0;
    background-color: lightgray;

    h3 {
        font-size: 20px;
        margin: 20px 0;
        color: $primary-color;
    }

    h1 {
        font-size: 50px;
        margin: 20px 0;

        span {
            color: #20ad96;
            font-weight: initial;
        }
    }

    .container {
        text-align: left;
        display: flex;
        flex-wrap: wrap;
        width: 80%;
        margin: 0 auto;

        .card {
            width: 50%;
            min-height: 50px;
            display: flex;
            padding: 20px;

            &:hover {
                border: 2px solid black;
                border-radius: 15px;
                background-color: antiquewhite;
            }
        }

        .card-img {
            width: 150px;
            height: 150px;


            img {
                width: 100%;
                height: 100%;
                display: block;
                border-radius: 50%;
            }
        }

        .card-text {
            min-height: 50px;
            margin-left: 20px;
            display: flex;
            flex-direction: column;
            justify-content: space-around;
            font-size: 20px;

            .price {
                color: #20ad96;
                font-weight: bold;
            }

            .text {
                font-weight: bold;
                width: 82%;
            }

            span {
                margin-right: 20px;
                color: $primary-color;

                i {
                    color: $primary-color;
                }
            }
        }
    }

    input {
        padding: 10px 30px;
        background-color: #20ad96;
        border: none;
        color: white;
        border-radius: 5px;
        margin: 30px 0;

        &:hover {
            background-color: #3f3a64;
            color: white;
        }
    }
}
</style>
