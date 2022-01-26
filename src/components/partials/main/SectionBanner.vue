<template>
    <section id="bnnr" class="banner">
        <div class="color-gradient d-flex flex-column justify-content-center align-items-center">
            <div class="row m-0">
                <div class="col">
                    <blockquote class="quote text-center">
                        “I’ve failed over and over again in my <br>
                            life. And that is why I succeed.” 
                    </blockquote>
                </div>
            </div>
            <div class="row m-0">
                <div class="col">
                    <svg class="vector-waves pt-3 pb-5" width="352" height="61" viewBox="0 0 352 61" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M5 51.5215L45 12.5215C48.6667 8.35485 58 2.52152 67.5 12.5215C77 22.5215 97 42.6882 108 51.5215C110.833 53.1882 117.5 55.5215 121.5 51.5215C125.5 47.5215 150.167 23.8549 162 12.5215C165.5 8.35485 175.3 2.52152 186.5 12.5215C197.7 22.5215 216.167 42.6882 224 51.5215C227 53.6882 234.5 56.7215 240.5 51.5215C246.5 46.3215 269.333 23.3549 280 12.5215C283 8.85485 291.9 3.72152 303.5 12.5215C315.1 21.3215 338.667 44.6882 347 54.0215" stroke="#FFF941" stroke-width="13"/>
                    </svg>
                </div>
            </div>
            <div class="row m-0 mb-2 justify-content-center">
                <div class="col-8">
                    <p class="sub-quote"> Arcu auctor gravida nisl, congue sit nisi tincidunt eget proin. In lacinia lacus donec sed massa in ipsum eros, tristique. Gravida suspendisse etiam in iaculis </p>
                </div>
            </div>
            <div class="row m-0 pt-2">
                <div class="col">
                    <a href="#" class="buy-banner d-inline-block text-decoration-none rounded-pill">Buy Avada today <i class="fas fa-angle-right"></i> </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "SectionBanner"
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .banner {
        background-image: url('../../../assets/img/banner2-2x.jpg');
        background-position: center;
        background-size: cover;
        width: 100%;
        height: 775px;

        .color-gradient {
            background: linear-gradient(0deg, rgba(1,3,18,1) 0%, rgba(1,3,18,0.14329481792717091) 100%);
            width: 100%;
            height: 775px;

            .row {

                .col {

                    .quote {
                        color: #ffffff;
                        font-weight: 500;
                        font-size: 3.5em;
                    }
                    .vector-waves {
                        width: 80px;
                        height: auto;
                    }
                    .buy-banner {
                            background-color: $dodgerBlue;
                            transition: background-color 0.25s;
                            color:white;
                            font-size: 1.1em;
                            font-weight: 500;
                            padding: 0.7em 2.5em;

                            &:hover { 
                                background-color: #FF414B; 
                                cursor: pointer;    
                            }
                        }
                }
                .col-8 {
                    .sub-quote {
                        text-align: center;
                        color: #ffffff;
                        font-size: 1.5em;
                    }
                }
            }
        }
    }
</style>