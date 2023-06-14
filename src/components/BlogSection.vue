<script>
export default {
    name: "BlogSection",
    data() {
        return {
            listBlogs: [
                {
                    id: 1,
                    img: "../../public/images/artist-blog-03-480x325.jpeg",
                    text: "Brush Strokes Energize Trees in Paintings",
                    data: "May 15, 2020",
                    wiews: "688 wiews"
                },
                {
                    id: 2,
                    img: "../../public/images/artist-blog-01-480x325.jpg",
                    text: "Pocket-Sized Notebooks Hold Miniature Paintings",
                    data: "May 15, 2020",
                    wiews: "603 wiews"
                },
                {
                    id: 3,
                    img: "../../public/images/artist-blog-02-480x325.jpg",
                    text: "Connection Between Self- Portraits and Identity",
                    data: "May 15, 2020",
                    wiews: "397 wiews"
                },

            ]
        }
    }
}

</script>

<template>
    <section class="blog">
        <h3>
            ENJOY READING ON MAXCOACH
        </h3>
        <h1>
            Latest on <span>Our Blogs</span>
        </h1>
        <div class="container">
            <div class="card" v-for="elm in listBlogs">
                <div class="card-img">
                    <img :src="elm.img" alt="">
                </div>
                <div class="artist">
                    ARTIST
                </div>
                <div class="card-text">
                    {{ elm.text }}
                </div>
                <div>
                    <span>
                        <i class="fa-regular fa-calendar" style="color: #808080;"></i>
                        {{ elm.data }}
                    </span>
                    <span>
                        <i class="fa-solid fa-eye" style="color: #808080;"></i>
                        {{ elm.wiews }}
                    </span>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

.blog {
    min-height: 50px;
    padding: 50px 0;
    background-color: lightgray;

    h3 {
        font-size: 20px;
        margin: 20px 0;
        color: $primary-color;
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
        width: 70%;
        margin: 0 auto;
        min-height: 50px;
        display: flex;

        .card {
            width: calc(100% / 3 - 40px);
            min-height: 50px;
            margin: 20px;

            .card-img img {
                width: 100%;
                display: block;
            }

            .card-text {
                font-weight: bold;
                font-size: 18px;
            }

            div {
                margin-top: 20px;
            }

            .artist {
                font-weight: bold;
                color: $primary-color;
            }

            span {
                margin-right: 20px;
                color: $primary-color;
            }
        }
    }
}</style>
