<template>
    <section class="training position-relative">
        <div class="girl-abs position-absolute">
            <div class="color-gradient">
                <div class="play-button rounded-circle position-absolute">
                    <i class="fas fa-play"></i>
                </div>
            </div>
        </div>
        <div class="row m-0">
            <div class="col-5 offset-6 d-flex flex-column">
                <h3>Tune up your workouts</h3>
                <h1>The best health &amp; fitness advice online</h1>
                <a class="yt-theme-f d-flex text-decoration-none">
                    <img class="theme-f-logo" src="../../../assets/img/unnamed.jpg" alt="">
                    <div class="theme-f-text">
                        <small>ThemeFusion</small>
                        <div class="link d-flex">
                            <div class="yt">
                                <span> <i class="fab fa-youtube"></i> YouTube </span>
                            </div>
                            <div class="subs">
                                <small>999 &plus;</small>
                            </div>
                        </div>
                    </div>
                </a>
                <p> Arcu eu facilisi ut quisque placerat nunc habitant. Magna semper mauris, venenatis, leo integer sit pellentesque. </p>
                <a class="yt-btn text-decoration-none rounded-pill" href="#"> <i class="fab fa-youtube"></i> Visit my YouTube channel </a>
            </div>
        </div>
        <div class="container-xxl d-flex flex-column justify-content-end p-0 pb-3">
            <div class="row m-0 pb-5">
                <div class="col p-0 d-flex">
                    <h3>Featured playlists</h3>
                </div>
                <div class="col p-0">
                    <h5 class="text-end">View all videos <i class="fas fa-angle-right"></i> </h5>
                </div>
            </div>
            <div class="row justify-content-between m-0 p-0 pb-5">
                
                <div v-for="(el, index) in train"
                    :key="el + index"
                    class="training-card d-flex flex-column align-items-center p-0">
                    <div 
                        class="container-img position-relative"
                        :class="el.id">
                        <div class="play-button rounded-circle position-absolute">
                            <i class="fas fa-play"></i>
                        </div>
                    </div>
                    <h4>{{ el.title_training }}</h4>
                    <h5>{{ el.caption_training }}</h5>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "SectionTraining",
        props: [ 'train' ],
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .training {
        background-color: #ffffff;
        width: 100%;
        height: 150vh;

        .girl-abs {
            background-image: url('../../../assets/img/service15-2x.jpg');
            background-position: center;
            background-size: cover;
            overflow: hidden;
            border-radius: 4px;
            border-bottom-right-radius: 50px;
            top: -60px;
            left: 0;
            width: 934px;
            height: 785px;

            .color-gradient {
                background: linear-gradient(0deg, rgba(0,0,0,0.5074404761904762) 0%, rgba(0,0,0,0) 60%);
                width: 100%;
                height: 100%;

                .play-button {
                    background-color: #FFFFFF;
                    color: $dodgerBlue;
                    text-align: center;
                    width: 6em;
                    line-height: 6em;
                    height: 6em;
                    top: 50%;
                    right: 50%;
                    transform: translate(50%,-50%);
    
                    .fas.fa-play { font-size: 1.2em; }
                }
            }
        }
        .row {

            .col-5 {
                padding: 6rem;

                h3 {
                    color: $dodgerBlue;
                    margin-bottom: 1em;
                }
                h1 {
                    font-size: 3.8em;
                    margin-bottom: 0.6em;
                }
                .yt-theme-f {
                    margin-bottom: 2em;
                   
                    .theme-f-text {
                        padding-left: 0.8em;

                        small {
                            color: #555555;
                        }
                        .link {

                            .yt {
                                background-color: #E62117;
                                color: #ffffff;
                                padding: 0 0.3em;
                            }
                            .subs {
                                background-color: #fafafa;
                                color: #555555;
                                border: 1px solid #d1d0d0;
                                padding: 0 0.3em;
                            }
                        }
                    }
                }
                p {
                    font-size: 1.4em;
                    color: #524A59;
                    margin-bottom: 1.7em;
                }
                .yt-btn {
                    background-color: #ff0000;
                    color: #ffffff;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    font-size: 1.1em;
                    font-weight: 500;
                    width: 280px;
                    height: 3.2em;

                    .fab.fa-youtube {
                        padding-right: 0.5em;
                    }

                }
            }
        }
        .container-xxl {
            height: 713px;

            // .row {
            //     .col {}
            //     .col {}
            // }
            .row {
                .training-card {
                    width: 410px;
                    height: 410px;

                    .container-img {
                        background-size: cover;
                        border-radius: 4px;
                        border-bottom-right-radius: 40px;
                        width: 410px;
                        height: 250px;

                        .play-button {
                            background-color: #FFFFFF;
                            color: $dodgerBlue;
                            text-align: center;
                            width: 4em;
                            line-height: 4em;
                            height: 4em;
                            top: 50%;
                            right: 50%;
                            transform: translate(50%,-50%);
            
                            .fas.fa-play { 
                                font-size: 0.7em;
                                padding-left: 0.3em;
                            }
                        }
                    }
                    .container-img.a { background-image: url('../../../assets/img/video2-2x.jpg'); }
                    .container-img.b { background-image: url('../../../assets/img/video7-2x.jpg'); }
                    .container-img.c { background-image: url('../../../assets/img/video9-2x.jpg'); }
                    h4 { padding-top: 1.5em;}
                    h5 { color: $dodgerBlue; }
                }
            }

        }

    }

</style>