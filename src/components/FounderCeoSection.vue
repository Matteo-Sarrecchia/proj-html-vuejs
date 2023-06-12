<script>
export default {
    name: "FounderCeoSection"
}
</script>

<template>
    <section class="founderCeo">
        <h2>
            Let passion and determination be the guide along the way and develop at your own pace that's comfortable.
        </h2>
        <div>
            FANNIE MORENO
        </div>
        <div>
            /Founder & CEO
        </div>

        <div class="container">
            <div class="col">
                <div class="text-number">1.926</div>
                <div class="text">FINISHED SESSIONS</div>
            </div>
            <div class="col">
                <div class="text-number">3.092+</div>
                <div class="text">ENROLLED LEARNERS
                </div>
            </div>
            <div class="col">
                <div class="text-number">200</div>
                <div class="text">ONLINE INSTRUCTORS
                </div>
            </div>
            <div class="col">
                <div class="text-number">100%</div>
                <div class="text">SATISFACTION RATE
                </div>
            </div>

        </div>
    </section>
</template>

<style lang="scss" scoped>
@use "../styles/generals.scss" as *;

.founderCeo {
    border: 1px solid rgb(249, 7, 7);
    min-height: 50px;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    // default background
    background-color: lightseagreen;

    h2,
    div {
        width: 50%;
        margin-bottom: 20px;
    }

    h2 {
        margin: 30px;
        margin-top: 50px;
        font-size: 35px;
    }

    .container {
        display: flex;
        justify-content: center;
        margin-top: 50px;
        width: 80%;

        .col {
            width: 25%;
            min-height: 50px;
            display: flex;
            flex-direction: column;
            align-items: center;

            div {
                padding: 10px;
                margin: 0;
            }

            .text-number {
                font-size: 40px;
                color: green;
                font-weight: bolder;
            }

            .text {
                width: 100%;
            }
        }
    }
}
</style>
