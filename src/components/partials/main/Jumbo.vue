<template>
    <div class="jumbo-container-photo">
        <div class="container-gradient position-relative">
            <div class="container-xxl d-flex justify-content-between align-items-center p-0">
                <div class="row m-0 align-items-center">
                    <div class="col-7 p-0">
                        <h3 class="h3-certified">Certified fitness professional</h3>
                        <!-- <h1 class="h1-title"> <span class="yellow-spacer">Ta</span>ke control of your health</h1> -->
                        <h1 class="h1-title"> Take control of your health</h1>
                        <svg class="vector-waves" width="352" height="61" viewBox="0 0 352 61" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M5 51.5215L45 12.5215C48.6667 8.35485 58 2.52152 67.5 12.5215C77 22.5215 97 42.6882 108 51.5215C110.833 53.1882 117.5 55.5215 121.5 51.5215C125.5 47.5215 150.167 23.8549 162 12.5215C165.5 8.35485 175.3 2.52152 186.5 12.5215C197.7 22.5215 216.167 42.6882 224 51.5215C227 53.6882 234.5 56.7215 240.5 51.5215C246.5 46.3215 269.333 23.3549 280 12.5215C283 8.85485 291.9 3.72152 303.5 12.5215C315.1 21.3215 338.667 44.6882 347 54.0215" stroke="#FFF941" stroke-width="13"/>
                        </svg>
                        <p class="p-curabitur mb-5">Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet.</p>
                        <a href="#" class="yt-jumbo text-decoration-none rounded-pill"> <i class="fab fa-youtube"></i> Visit my YouTube channel </a> <a href="#" class="buy-jumbo text-decoration-none rounded-pill">Buy Avada today <i class="fas fa-arrow-right"></i> </a>
                    </div>
                    <div class="col-5 p-0 position-relative">
                        <div class="play-button rounded-circle position-absolute">
                            <i class="fas fa-play"></i>
                        </div>
                    </div>
                </div>
            </div>
            <div class="demos position-absolute d-flex flex-column justify-content-evenly align-items-center">
                <svg class="fss-before" width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M26 5.99994H6C5.44772 5.99994 5 6.44765 5 6.99994C5 7.55222 5.44772 7.99994 6 7.99994H26C26.5523 7.99994 27 7.55222 27 6.99994C27 6.44765 26.5523 5.99994 26 5.99994Z"></path>
                    <path d="M24 2.99994H8C7.44772 2.99994 7 3.44765 7 3.99994C7 4.55222 7.44772 4.99994 8 4.99994H24C24.5523 4.99994 25 4.55222 25 3.99994C25 3.44765 24.5523 2.99994 24 2.99994Z"></path>
                    <path fill-rule="evenodd" clip-rule="evenodd" d="M3 12.9999C3 10.7908 4.79086 8.99994 7 8.99994H25C27.2091 8.99994 29 10.7908 29 12.9999V24.9999C29 27.2091 27.2091 28.9999 25 28.9999H7C4.79086 28.9999 3 27.2091 3 24.9999V12.9999ZM11.2142 23.9962C11.0575 23.9962 10.9524 23.8414 11.0218 23.7026L15.8007 14.1131C15.8761 13.9623 16.0883 13.9623 16.1637 14.1131L16.5247 14.8371C18.9529 19.7192 15.6459 24.0041 11.2142 23.9962ZM18.3797 19.2906C18.4531 19.1399 18.6674 19.1399 18.7428 19.2906L20.9785 23.7065C21.0459 23.8414 20.9467 24.0001 20.796 24.0001H18.8578C17.4335 24.0001 16.6896 22.6194 17.2807 21.4371L18.3797 19.2906Z"></path>
                </svg>
                <h6 class="text-demos"> <small> Demos </small></h6>
            </div>
            <div class="on-sale position-absolute d-flex flex-column justify-content-evenly align-items-center">
                <div class="on-sale-price"> <span class="dollar"> &#36; </span> 39 </div>
                <h6 class="text-demos"> <small> On Sale </small></h6>
            </div>
        </div>
        
    </div>
</template>

<script>
    export default {
        name: "Jumbo"
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .jumbo-container-photo {
        background-image: url('../../../assets/img/slider82x-scaled.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        width: 100%;
        height: 675px;

        .container-gradient {
            background: linear-gradient(90deg, rgba(6,6,8,1) 44%, rgba(4,9,12,0.773546918767507) 52%, rgba(3,11,14,0.5186449579831933) 62%, rgba(2,13,17,0) 74%);
            width: 100%;
            height: 675px;

            .container-xxl {
                // border: 3px solid red;
                height: 675px;

                .row {
                    width: 100%;
                    height: 100%;

                    .col-7 {

                        .h3-certified {
                            color: #FF414B;
                        }
                        .h1-title {
                            color: white;
                            font-size: 4.5em;
                            margin-bottom: 0.5em;

                            .yellow-spacer {
                                border-bottom: 5px solid #F1EC3E;
                                border-radius: 5px;
                                padding-bottom: 0.3em
                            }
                        }
                        .vector-waves {
                            width: 80px;
                            height: auto;
                            margin-bottom: 1.3em
                        }
                        .p-curabitur {
                            color: #93939f;
                            font-size: 1.5em;
                        }
                        .yt-jumbo {
                            background-color: $dodgerBlue;
                            color:white;
                            font-size: 1.2em;
                            padding: 0.9em 1.8em;

                            &:hover {
                                color: white;
                            }
                        }
                        .buy-jumbo {
                            color:#D2D2C5;
                            border: 3px solid #2C2A35;
                            font-size: 1.2em;
                            padding: 0.9em 1.8em;
                            margin-left: 1em;
                            i { margin-left: 0.2em; }

                            &:hover {
                                color: #D2D2C5;
                            }
                            
                        }
                        
                    }
                    .col-5 {
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
            }
            .demos {
                background-color: white;
                top: 50px;
                right: 20px;
                width: 66px;
                height: 66px;
                border-radius: 0.5em;
                padding-top: 0.4em;
                .fss-before { fill: #33475b; }
                .text-demos {
                    display: block;
                    color: #33475b;
                }
            }
            .on-sale {
                background-color: white;
                top: 122px;
                right: 20px;
                width: 66px;
                height: 66px;
                border-radius: 0.5em;
                padding-top: 0.2em;

                .on-sale-price {
                    font-size: 1.8em;
                    font-weight: 700;
                    color: #65BC7B;

                    .dollar {
                        font-size: 0.6em;
                        vertical-align: text-top;
                    }
                }
            }
        }
    }
</style>