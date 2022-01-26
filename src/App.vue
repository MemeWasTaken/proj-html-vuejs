<template>
    <div id="app">
        <div class="container-fluid p-0">
            <Header 
                :nav="results.navigate"
            />
            <Main 
                :chall="results.challenges"
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
                            "link_navigate": "#",
                            "isActive": true,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Services",
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "About",
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Videos",
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Blog",
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Store",
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": true,
                            "isButton": false,
                        },
                        {
                            "text_link_navigate": "Schedule a workout",
                            "link_navigate": "#",
                            "isActive": false,
                            "isNew": false,
                            "isButton": true,
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