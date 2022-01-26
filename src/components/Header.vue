<template>
    <header id="hdr">
        <div class="container-xxl d-flex justify-content-between align-items-center p-0">
            <Logo />
            <Navbar
                :nav="navb"
            />
        </div>
    </header>
</template>

<script>
    import Logo from "./partials/header/Logo.vue"
    import Navbar from "./partials/header/Navbar.vue"
    
    export default {
        name: "Header",
        components: {
            Logo,
            Navbar,
        },
        data() { return { "navb": this.nav } },
        props: [ 'nav' ],
    }
</script>

<style lang="scss" scoped>
    @import '../assets/scss/style.scss';
    
    header {
        background-color: $codGray;
        height: 100px;

        .container-xxl {
            height: 100px;
        }
    }
</style>