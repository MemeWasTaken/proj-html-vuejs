<template>
    <div class="upper-footer">
        <div class="container-xxl p-0">
            <div class="row m-0 p-0">
                <div class="col-4 a d-flex flex-column justify-content-start align-items-center m-0 p-0">
                    <img src="../../../assets/img/logo-2x.png" alt="">
                    <p class="pt-5"> Ac aliquam neque sagittis diam faucibus vitae purus turpis phasellus. Pellentesque consectetur amet purus ultrices mauris. </p>
                    <div class="socials d-flex justify-content-between pt-4">
                        <a class="text-decoration-none" href=""> <i class="fab fa-facebook-f"></i> </a>
                        <a class="text-decoration-none" href=""> <i class="fab fa-twitter"></i> </a>
                        <a class="text-decoration-none" href=""> <i class="fab fa-youtube"></i> </a>
                        <a class="text-decoration-none" href=""> <i class="fab fa-instagram"></i> </a>
                        <a class="text-decoration-none" href=""> <i class="fab fa-linkedin-in"></i> </a>
                    </div>
                </div>
                <div class="col-4 b d-flex flex-column justify-content-start align-items-center m-0 p-0">
                    <h5 class="text-uppercase">Recent Posts</h5>
                    <ul class="list-unstyled d-flex flex-column justify-content-center align-items-center">
                        <li> <a class="text-decoration-none" href="#"> <i class="fas fa-angle-right"></i> The best protein shake </a> </li>        
                        <li> <a class="text-decoration-none" href="#"> <i class="fas fa-angle-right"></i> Ultimate cardio workout </a> </li>        
                        <li> <a class="text-decoration-none" href="#"> <i class="fas fa-angle-right"></i> New juices available now </a> </li>        
                        <li> <a class="text-decoration-none" href="#"> <i class="fas fa-angle-right"></i> Tips to find training partners </a> </li>        
                        <li> <a class="text-decoration-none" href="#"> <i class="fas fa-angle-right"></i> 20 best healthy recipes </a> </li>        
                    </ul>
                </div>
                <div class="col-4 c d-flex flex-column justify-content-start align-items-center m-0 p-0">
                    <h5 class="text-uppercase">Contact Informations</h5>
                    <ul class="list-unstyled d-flex flex-column justify-content-center align-items-center">
                        <li class="adress"> 4746 Tipple Road Michigan 48449 </li>
                        <li> Mobile : 1.800.000.0000 </li>
                        <li> Email : info@your-company.com </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "UpperFooter"
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .upper-footer {
        background-color: #060607;
        width: 100%;
        height: 560px;
        .container-xxl {
            
            .row {
                // border: 1px solid $dodgerBlue;
                width: 100%;
                height: 560px;
                .col-4 {
                    // border: 1px solid lightblue;
                    padding-top: 9em !important;
                }
                .col-4.a {

                    img {
                        width: 220px;
                        height: auto;
                    }
                    p {
                        color: #CFCED1;
                        text-align: center;
                        font-size: 1.2em;
                        padding: 0 1.8em;
                    }
                    .socials {
                        width: 35%;
                        a {
                            color: #FF414B;
                            font-size: 1.2em;
                        }
                    }
                }
                .col-4.b {

                    h5 { color: #ffffff; }
                    ul {

                        li {

                            padding: 0.8em 0 !important;
                            a {
                                color: #ffffff;
                                font-size: 1.2em;
                            }
                        }
                    }
                }
                .col-4.c {
                    h5 { color: #ffffff; }
                    ul {

                        li {
                            color: #ffffff;
                            font-size: 1.2em;
                            padding: 0.3em 0 !important;
                        }
                        .adress {
                            color: #BCBBBE;
                            padding: 1em 0 !important;
                        }
                    }
                }
            }
        }
    }
</style>