<template>
    <div id="app">
        <div class="container-fluid p-0">
            <Header 
                :nav="results.navigate"
            />
            <Main 
                :chall="results.challenges"
                :train="results.trainings"
                :serv="results.services"
            />
            <Footer 
                :foot="results.recent_posts"
            />
        </div>
    </div>
</template>

<script>
    import Header from "./components/Header.vue"
    import Main from "./components/Main.vue"
    import Footer from "./components/Footer.vue"
 
    export default {
        name: "App",
        components: {
            Header,
            Main,
            Footer,
        },
        data() {
            return {
                "results": {
                    "navigate": [
                        {
                            "text_link_navigate": "Home",
                            "icon": null, 
                            "link_navigate": "#",
                            "isActive": true,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Services",
                            "icon": null, 
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "About",
                            "icon": null,
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Videos",
                            "icon": null,
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Blog",
                            "icon": null,
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Store",
                            "icon": null,
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": true,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Schedule a workout",
                            "icon": null,
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": true,
                        },
                        {
                            "text_link_navigate": null,
                            "icon": "shopping-cart",
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": null,
                            "icon": "search",
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                    ],
                    "recent_posts": [
                        {
                            "text_link_post": "The best protein shake",
                            "link_post": "#"
                        },
                        {
                            "text_link_post": "Ultimate cardio workout",
                            "link_post": "#"
                        },
                        {
                            "text_link_post": "New juices available now",
                            "link_post": "#"
                        },
                        {
                            "text_link_post": "Tips to find training partners",
                            "link_post": "#"
                        },
                        {
                            "text_link_post": "20 best healthy recipes",
                            "link_post": "#"
                        }
                    ],
                    "challenges": [
                        {
                            "poster_challenge": "../../../assets/img/service6-2x.jpg",
                            "title_challenge": "Crossfit workout",
                            "subtitle_challenge": "Push your limits",
                            "id": 'a'
                        },
                        {
                            "poster_challenge": "../../../assets/img/box1-2x.jpg",
                            "title_challenge": "New gym apparel",
                            "subtitle_challenge": "Look good, feel good",
                            "id": 'b'
                        },
                        {
                            "poster_challenge": "../../../assets/img/box3-2x.jpg",
                            "title_challenge": "Team training",
                            "subtitle_challenge": "Find a partner",
                            "id": 'c'
                        }
                    ],
                    "trainings": [
                        {
                            "poster_training": "../../../assets/img/video2-2x.jpg",
                            "title_training": "Thighs &amp; glute workout",
                            "caption_training": "Increase your mobility",
                            "id": "a"
                        },
                        {
                            "poster_training": "../../../assets/img/video7-2x.jpg",
                            "title_training": "Lift, firm &amp; perk up",
                            "caption_training": "Feel young again",
                            "id": "b"
                        },
                        {
                            "poster_training": "../../../assets/img/video9-2x.jpg",
                            "title_training": "Slim &amp; trim your waist",
                            "caption_training": "Shed those extra pounds",
                            "id": "c"
                        }
                    ],
                    "services": [
                        {
                            "img_service": "watch.png",
                            "title_service": "Team training",
                            "subtitle_service": "Find a partner",
                            "par_service": "Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus eget sed duis vehnicula. Tristique.",
                            "text_link_service": "Find a partner",
                            "link_service": "#",
                        },
                        {
                            "img_service": "handlebar.png",
                            "title_service": "Crossfit workout",
                            "subtitle_service": "Push your limits",
                            "par_service": "Vestibulum, curabitur eu sem nibh ultrices sit nulla adipiscing. Nisl sit fames amet senectus eget sed duis vehnicula. Tristique.",
                            "text_link_service": "Learn about crossfit",
                            "link_service": "#",
                        },
                        {
                            "img_service": "hips.png",
                            "title_service": "Weight loss plan",
                            "subtitle_service": "Shed those pounds",
                            "par_service": "At laoreet sebectus volutpat diam vel sed sed amet pellentesque. Lobortis ut aliquam risus purus. A tellus ut etiam.",
                            "text_link_service": "Schedule a workout",
                            "link_service": "#",
                        },
                    ],

                }
            }
        }
    };
</script>

<style lang="scss">
    @import '~bootstrap/scss/bootstrap.scss';
    @import './assets/scss/style.scss';

    #app {
        font-family: $fontFamily;
    }
</style>