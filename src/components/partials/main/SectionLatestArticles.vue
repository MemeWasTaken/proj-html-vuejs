<template>
    <section class="latest-articles">
        <div class="container-xxl d-flex flex-column justify-content-end">
            <div class="row m-0 pb-5">
                <div class="col p-0 d-flex">
                    <h3>Latest articles</h3>
                </div>
                <div class="col p-0">
                    <h5 class="text-end">Read all articles <i class="fas fa-angle-right"></i> </h5>
                </div>
            </div>
            <div class="row justify-content-between m-0 p-0">
                
                <div v-for="(el, index) in latarts"
                    :key="el + index"
                    class="article-card d-flex flex-column align-items-center p-0">
                    <div class="container-img position-relative"
                        :class="el.id">
                        <img :src="require(`../../../assets/img/${el.poster_article}`)" :alt="el.title_article">
                    </div>
                    <div class="article-info">
                        <h4 class="text-start"> {{ el.title_article }} </h4> 
                        <p class="text-start"> {{ el.subtitle_article }} </p>
                    </div>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: "SectionLatestArticles",
        props: [ 'latarts' ],
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .latest-articles {
        background-color: #ffffff;
        width: 100%;
        // height: 75vh;

        .container-xxl {
            // height: 713px;
            padding: 5.5em 0 4em 0;

            .row {
                .article-card {
                    width: 410px;
                    height: 410px;

                    .container-img {

                        img {
                            width: 410px;
                            height: 250px; 
                        }
                    }
                    .article-info {
                        width: 410px;
                        text-align: start;
                        padding: 1.5em 1.5em 0 1.5em ;

                        h4 { font-size: 1.6em; }
                        p { font-size: 1.1em; }
                    }
                }
            }
        }
    }
</style>