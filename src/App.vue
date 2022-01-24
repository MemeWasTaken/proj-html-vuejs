<template>
    <div id="app">
        <div class="container-fluid p-0">
            <Header></Header>
            <Main></Main>
            <Footer></Footer>
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
    };
</script>

<style lang="scss">
    @import '~bootstrap/scss/bootstrap.scss';
    @import './assets/scss/style.scss';

    #app {
        font-family: $fontFamily;
    }
</style>