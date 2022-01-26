<template>
    <section id="srvs" class="services-cards">
        <div class="container-xxl  p-0">
            <div class="row d-flex justify-content-between align-items-center m-0">

                <div v-for="(el, index) in serv"
                    :key="el + index" 
                    class="service-card d-flex flex-column justify-content-center align-items-center">
                    <img class="pb-3 " 
                        :src="require(`../../../assets/img/${el.img_service}`)"
                        :alt="el.title_service">
                    <h2 class="title"> {{ el.title_service }} </h2>
                    <h3 class="sub-title pb-4">{{ el.subtitle_service }}</h3>
                    <p class="par d-inline-block pt-3 pb-2"> {{ el.par_service }} </p>
                    <a class="a-link text-decoration-none" :href="link_service">
                        {{ el.text_link_service}} <i class="fas fa-angle-right"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "SectionServicesCards",
        props: [ 'serv' ],
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
                    transition: transform 0.3s;
                    border-radius: 10px;
                    width: 405px;
                    height: 550px;

                    &:hover { 
                        transform: scale(1.04);
                        cursor: pointer;
                    }
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