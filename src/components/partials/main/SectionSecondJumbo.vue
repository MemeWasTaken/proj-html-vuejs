<template>
    <section class="jumbo-container-photo">
        <div class="container-gradient position-relative">
            <div class="container-xxl d-flex justify-content-between align-items-center p-0">
                <div class="row m-0 align-items-center">
                    <div class="col-9 p-0">
                        <h3 class="h3-certified mt-5 pt-5">Join our mailing list today</h3>
                        
                        <h1 class="h1-title"> Insider offers &amp; flash sales in your inbox every week. </h1>
                        <svg class="vector-waves mb-3 d-block" width="352" height="61" viewBox="0 0 352 61" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path d="M5 51.5215L45 12.5215C48.6667 8.35485 58 2.52152 67.5 12.5215C77 22.5215 97 42.6882 108 51.5215C110.833 53.1882 117.5 55.5215 121.5 51.5215C125.5 47.5215 150.167 23.8549 162 12.5215C165.5 8.35485 175.3 2.52152 186.5 12.5215C197.7 22.5215 216.167 42.6882 224 51.5215C227 53.6882 234.5 56.7215 240.5 51.5215C246.5 46.3215 269.333 23.3549 280 12.5215C283 8.85485 291.9 3.72152 303.5 12.5215C315.1 21.3215 338.667 44.6882 347 54.0215" stroke="#FFF941" stroke-width="13"/>
                        </svg>
                        <input class="sub-email d-inline-block mt-5 border-0 rounded-pill mb-3" type="email" name="" id="" placeholder="Insert your email...*">
                        <a href="#" class="yt-jumbo d-inline-block text-decoration-none rounded-pill ms-5"> Subscribe </a>
                        <p class="p-curabitur mb-5 mt-5">Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet, consectetur adipiscing elit sed porttitor lectus.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "SectionSecondJumbo"
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';
    
    .jumbo-container-photo {
        background-image: url('../../../assets/img/banner1-2x.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        width: 100%;
        height: 731px;

        .container-gradient {
            background: linear-gradient(90deg, rgba(6,6,8,1) 44%, rgba(4,9,12,0.773546918767507) 52%, rgba(3,11,14,0.5186449579831933) 62%, rgba(2,13,17,0) 74%);
            width: 100%;
            height: 731px;

            .container-xxl {
                // border: 3px solid red;
                height: 675px;

                .row {
                    width: 100%;
                    height: 100%;

                    .col-9 {

                        .h3-certified {
                            color: #FF414B;
                        }
                        .h1-title {
                            color: white;
                            font-size: 4em;
                            margin-bottom: 0.5em;

                        }
                        .vector-waves {
                            width: 80px;
                            height: auto;
                            margin-bottom: 1.3em
                        }
                        .sub-email {
                            font-size: 1.2em;
                            padding: 0.7em 1.2em;
                            width: 670px;
                        }
                        .p-curabitur {
                            color: #93939f;
                            font-size: 1.5em;
                        }
                        .yt-jumbo {
                            background-color: $dodgerBlue;
                            transition: background-color 0.25s;
                            color:white;
                            font-size: 1.2em;
                            font-weight: 500;
                            padding: 0.7em 4em;

                            &:hover { 
                                background-color: #FF414B; 
                                cursor: pointer;    
                            }
                        }
                    }
                }
            }
        }
    }

</style>