<template>
    <nav class="navbar navbar-expand-lg navbar-trasparent bg-trasparent">
            <div class="navbar-nav">

                <a v-for="(el, index) in nav"
                    :key="el + index"
                    class="nav-link"
                    :class="getClass(el)"
                    :href="el.link_navigate">
                    
                    <span v-show="el.text_link_navigate"> {{ el.text_link_navigate }} </span>
                    <span v-show="el.isNew" class="new ms-1 ps-2 pe-2"> new </span>
                    <i v-show="el.icon"
                        class="fas"
                        :class="`fa-${el.icon}`">
                    </i>

                </a>

            </div>
    </nav>
</template>

<script>
    export default {
        name: "Navbar",
        props: [ 'nav' ],
        methods: {
            getClass(el) {
                if (el.isActive == true) { return "fs-5 text-white me-3";
                } else if (el.isButton == true) { return "btn-nav rounded-pill text-decoration-none";
                } else if (el.icon) { return "btn-nav search text-decoration-none";
                } else { return "fs-5 not-selected me-3"; }

            }
        },
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';
    
    .nav-link { &:hover { color: #ffffff; } }
    .new {
        background-color: #FFF941;
        color: #000000;
        font-size: 0.7em;
        padding-top: 0.3em;
        padding-bottom: 0.4em;
        border-radius: 3px  ;
    }
    .not-selected {
        color: #98939F;
    }
    .btn-nav {
        color: #98939F;
        font-size: 1em;
        padding-bottom: 0.8em;
        align-self: center;
        &:hover {
            color: white;
            cursor: pointer;
        }
    }
    .btn-nav.rounded-pill {
        background-color: $dodgerBlue;
        padding-top: 0.8em;
        padding-left: 2em !important;
        padding-right: 2em !important;
        font-weight: 500;
        margin-left: 2em;
        margin-right: 2em;
        font-size: 0.85em;
        color: #ffffff;
    }
    .btn-nav.search {
        margin-left: 1.2em;
    }
</style>