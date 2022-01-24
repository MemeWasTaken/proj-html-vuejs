<template>
    <div class="jumbo-container-photo">
        <div class="container-gradient">
            <div class="container-xxl d-flex justify-content-between align-items-center p-0">
                <div class="row m-0">
                    <div class="col-7 p-0">
                        <h3 class="h3-certified">Certified fitness professional</h3>
                        <h1 class="h1-title"> <span>Ta</span>ke control of your health</h1>
                        <p>Curabitur non nulla sit amet nisl tempus convallis quis ac lectus dolor sit amet.</p>
                        <a href="#"> <i class="fab fa-youtube"></i> Visit my YouTube channel </a> <a href="#">Buy Avada today <i class="fas fa-arrow-right"></i> </a>
                    </div>
                    <div class="col-5 p-0">

                    </div>
                </div>
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
    .jumbo-container-photo {
        background-image: url('../../../assets/img/slider82x-scaled.jpg');
        background-size: cover;
        background-repeat: no-repeat;
        width: 100%;
        height: 675px;

        .container-gradient {
            background: linear-gradient(90deg, rgba(6,6,8,1) 45%, rgba(4,9,12,0.773546918767507) 51%, rgba(3,11,14,0.5186449579831933) 57%, rgba(2,13,17,0) 64%);
            width: 100%;
            height: 675px;

            .container-xxl {
                border: 3px solid red;
                height: 675px;

                .row {
                    width: 100%;

                    .col-7 {

                        .h3-certified {
                            color: #BC0428;
                        }
                        .h1-title {
                            color: white;
                            font-size: 4.5em;
                        }
                        
                    }
                }
            }
        }
    }
</style>