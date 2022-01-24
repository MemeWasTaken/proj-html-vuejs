<template>
    <nav class="navbar navbar-expand-lg navbar-trasparent bg-trasparent">
        <a href="#" class="navbar-brand text-white me-3">Home</a>
        <div class="collapse navbar-collapse text-white" id="navbarNavAltMarkup">
            <div class="navbar-nav">
                <a href="#" class="nav-link fs-5 disabled me-3" aria-current="page">Services</a>
                <a href="#" class="nav-link fs-5 disabled me-3">About</a>
                <a href="#" class="nav-link fs-5 disabled me-3">Videos</a>
                <a href="#" class="nav-link fs-5 disabled me-3">Blog</a>
                <a href="#" class="nav-link fs-5 disabled me-3">Store <span class="new ms-1 ps-2 pe-2">new</span> </a> 
                <a href="#" class="nav-link btn-nav rounded-pill text-decoration-none ps-4 pe-4">Schedule a workout</a>
                <a href="#" class="nav-link btn-nav cart text-decoration-none"><i class="fas fa-shopping-cart"></i></a>
                <a href="#" class="nav-link btn-nav search text-decoration-none"><i class="fas fa-search"></i></a>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        name: "Navbar",
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';
    
    .new {
        background-color: #FFF941;
        color: #000000;
        font-size: 0.7em;
        padding-top: 0.3em;
        padding-bottom: 0.4em;
        border-radius: 3px  ;
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