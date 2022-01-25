<template>
    <section class="services-cards">
        <div class="container-xxl  p-0">
            <div class="row d-flex justify-content-between align-items-center m-0">
                <div class="service-card d-flex flex-column justify-content-center align-items-center">
                    <img class="pb-3 " src="../../../assets/img/watch.png" alt="">
                    <h2 class="title">Team training</h2>
                    <h3 class="sub-title pb-4">Find a partner</h3>
                    <p class="par d-inline-block pt-3 pb-2">Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus eget sed duis vehnicula. Tristique.</p>
                    <a class="a-link text-decoration-none" href="">Find a partner <i class="fas fa-angle-right"></i> </a>
                </div>
                <div class="service-card d-flex flex-column justify-content-center align-items-center">
                    <img class="pb-3 " src="../../../assets/img/handlebar.png" alt="">
                    <h2 class="title">Crossfit workout</h2>
                    <h3 class="sub-title pb-4">Push your limits</h3>
                    <p class="par d-inline-block pt-3 pb-2">Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus eget sed duis vehnicula. Tristique.</p>
                    <a class="a-link text-decoration-none" href="">Learn about crossfit <i class="fas fa-angle-right"></i> </a>
                </div>
                <div class="service-card d-flex flex-column justify-content-center align-items-center">
                    <img class="pb-3 " src="../../../assets/img/hips.png" alt="">
                    <h2 class="title">Weight loss plan</h2>
                    <h3 class="sub-title pb-4">Shed those pounds</h3>
                    <p class="par d-inline-block pt-3 pb-4">At laoreet sebectus volutpat diam vel sed sed amet pellentesque. Lobortis ut aliquam risus purus. A tellus ut etiam.</p>
                    <a class="a-link text-decoration-none" href="">Schedule a workout <i class="fas fa-angle-right"></i> </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "SectionServicesCards"
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .services-cards {
        background-color: #060607;
        width: 100%;
        padding: 7.5em 0;
        // height: 750px;

        .container-xxl {

            .row {

                .service-card {
                    border: 5px solid #3240C1;
                    border-radius: 10px;
                    width: 405px;
                    height: 550px;

                    .title {
                        color: #ffffff;
                        font-size: 1.8em;
                    }
                    .sub-title {
                        color: #fff941;
                        font-size: 1.6em;
                    }
                    .par {
                        color: #CFCAD0;
                        text-align: center;
                        font-size: 1.2em;
                        width: 310px;
                    }
                    .a-link {
                        color: #ffffff;
                        font-size: 1.1em;
                        font-weight: 500;

                        .fas.fa-angle-right {
                            margin-left: 0.5em;
                        }
                    }

                }
            }
        }
    }
</style>