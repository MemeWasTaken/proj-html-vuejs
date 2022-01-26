<template>
    <section class="Challenge position-relative d-flex flex-column justify-content-end align-items-center">

        <div v-for="(el, index) in chall"
            :key="index" 
            class="challenge-card position-absolute"
            :class="el.id">
            <a class="text-decoration-none" :href="el.link_challenge">
                <div class="color-gradient-card d-flex flex-column justify-content-end ps-5 pb-4">
                    <svg class="vector-waves" width="352" height="61" viewBox="0 0 352 61" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M5 51.5215L45 12.5215C48.6667 8.35485 58 2.52152 67.5 12.5215C77 22.5215 97 42.6882 108 51.5215C110.833 53.1882 117.5 55.5215 121.5 51.5215C125.5 47.5215 150.167 23.8549 162 12.5215C165.5 8.35485 175.3 2.52152 186.5 12.5215C197.7 22.5215 216.167 42.6882 224 51.5215C227 53.6882 234.5 56.7215 240.5 51.5215C246.5 46.3215 269.333 23.3549 280 12.5215C283 8.85485 291.9 3.72152 303.5 12.5215C315.1 21.3215 338.667 44.6882 347 54.0215" stroke="#ffffff" stroke-width="13"/>
                    </svg>
                    <h2 class="text-white pt-4">{{ el.title_challenge }}</h2 >
                    <h3 class="subtitle-yellow">{{ el.subtitle_challenge}}</h3>
                </div>
            </a>
        </div>

        <div class="row m-0">
            <div class="col">
                <blockquote class="quote text-center">
                    “How you respond to the challenge in the second half <br>
                        will determine what you become after the game, <br>
                            whether you are a winner or a loser.” 
                </blockquote>
            </div>
        </div>
        <div class="row m-0">
            <div class="col">
                <svg class="vector-waves pt-3 pb-3" width="352" height="61" viewBox="0 0 352 61" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M5 51.5215L45 12.5215C48.6667 8.35485 58 2.52152 67.5 12.5215C77 22.5215 97 42.6882 108 51.5215C110.833 53.1882 117.5 55.5215 121.5 51.5215C125.5 47.5215 150.167 23.8549 162 12.5215C165.5 8.35485 175.3 2.52152 186.5 12.5215C197.7 22.5215 216.167 42.6882 224 51.5215C227 53.6882 234.5 56.7215 240.5 51.5215C246.5 46.3215 269.333 23.3549 280 12.5215C283 8.85485 291.9 3.72152 303.5 12.5215C315.1 21.3215 338.667 44.6882 347 54.0215" stroke="#FFF941" stroke-width="13"/>
                </svg>
            </div>
        </div>
        <div class="row m-0">
            <div class="col">
                <div class="brad-j d-flex align-items-center">
                    <img class="img-brad rounded-circle" src="../../../assets/img/avatar-1-2x.jpg" alt="">
                    <h5 class="name-brad"> Brad Johnson </h5>
                    <h5 class="city-brad"> Las Vegas </h5>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "SectionChallenge",
        props: [ 'chall' ],
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .Challenge {
        background: linear-gradient(152deg, rgba(6,24,230,1) 21%, rgba(85,15,148,1) 43%, rgba(158,6,69,1) 68%, rgba(211,0,13,1) 100%);
        width: 100%;
        height: 110vh;

        .challenge-card {
            width: 406px;
            height: 436px;
            border-radius: 5px;
            border-bottom-right-radius: 50px;
            top: -82px;
            transition: transform 0.3s;
            overflow: hidden;

            &:hover {
                transform: scale(1.04);
                cursor: pointer;
            }
            .color-gradient-card {
                background: linear-gradient(0deg, rgba(0,0,0,0.7203256302521008) 0%, rgba(0,0,0,0) 66%);
                width: 406px;
                height: 436px;
                .vector-waves {
                    width: 40px;
                    height: auto;
                }
                .subtitle-yellow { color: #fff941; }
            }
        }
        .challenge-card.a {
            background-image: url('../../../assets/img/service6-2x.jpg');
            background-size: cover;
            left: 280px;
        }
        .challenge-card.b {
            background-image: url('../../../assets/img/box1-2x.jpg');
            background-size: cover;
            left: 740px;
        }
        .challenge-card.c {
            background-image: url('../../../assets/img/box3-2x.jpg');
            background-size: cover;
            left: 1200px;
        }
        .row {
            .col {
                .quote {
                    color: #ffffff;
                    font-weight: 500;
                    font-size: 3em;
                }
                .vector-waves {
                    width: 80px;
                    height: auto;
                }
                .brad-j {
                    padding-bottom: 12em;
                    .img-brad {
                        width: 60px;
                        height: 60px;
                    }
                    .name-brad {
                        color: #ffffff;
                        padding: 0 1em;
                    }
                    .city-brad { color: #D7ACC8; }
                }
            }
        }
    }


</style>