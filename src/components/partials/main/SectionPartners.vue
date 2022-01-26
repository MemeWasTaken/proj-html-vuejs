<template>
    <section class="partners">
        <div class="container-xxl d-flex p-0">
            <div class="row justify-content-between align-items-center m-0 p-0">
                
                <div v-for="(el, index) in parts"
                    :key="el + index"
                    class="course-card d-flex flex-column justify-content-center align-items-center">
                    <img class="mb-3" :src="require(`../../../assets/img/${el.logo_partner}`)">
                    <svg class="vector-waves mb-4" width="352" height="61" viewBox="0 0 352 61" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M5 51.5215L45 12.5215C48.6667 8.35485 58 2.52152 67.5 12.5215C77 22.5215 97 42.6882 108 51.5215C110.833 53.1882 117.5 55.5215 121.5 51.5215C125.5 47.5215 150.167 23.8549 162 12.5215C165.5 8.35485 175.3 2.52152 186.5 12.5215C197.7 22.5215 216.167 42.6882 224 51.5215C227 53.6882 234.5 56.7215 240.5 51.5215C246.5 46.3215 269.333 23.3549 280 12.5215C283 8.85485 291.9 3.72152 303.5 12.5215C315.1 21.3215 338.667 44.6882 347 54.0215" stroke="#4154FF" stroke-width="13"/>
                    </svg>
                    <p class="text-center"> {{ el.par_partner }} </p>
                    <a class="text-decoration-none" :href="el.link_partner"> {{ el.text_link_partner }} <i class="fas fa-angle-right"></i> </a>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "SectionPartners",
        props: [ 'parts' ],
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .partners {
        background-color: #ffffff;
        width: 100%;
        height: 550px;

        .container-xxl {
            width: 100%;
            height: 550px;

            .row {
                width: 100%;

                .course-card {
                    // border: 1px solid blue;
                    width: 320px;
                    height: 320px;

                    &:hover {
                        cursor: pointer;
                    }
                    img {
                        width: 180px;
                        height: auto;
                    }
                    .vector-waves {
                        width: 40px;
                        height: auto;
                    }
                    p.text-center {
                        color: #574A59;
                        font-size: 1.2em;
                    }
                    a.text-decoration-none {
                        color: #000000;
                        font-weight: 500;
                        font-size: 1.1em;
                    }
                }
            }
        }
    }
</style>