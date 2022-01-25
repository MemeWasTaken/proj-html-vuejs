<template>
    <div class="bottom-footer d-flex justify-content-center align-items-center position-relative">
        <p class="m-0"> &copy; Copyright 2012 &hyphen; 2022 &vert; Avada Theme by <span class="text-white"> ThemeFusion </span> &vert; All Rights Reserved &vert; Powered by <span class="text-white"> WordPress </span> </p>
        <a class="text-decoration-none position-absolute d-flex" href="#">
            <i class="fas fa-chevron-up"></i>
        </a>
    </div>
</template>

<script>
    export default {
        name: "BottomFooter"
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .bottom-footer {
        background-color: #060607;
        border-top: 1px solid #252526;
        width: 100%;
        height: 110px;
        
        p {
            color: #98939F;
            font-size: 1.05em;
        }
        a {
            background-color: #2F2F2F;
            color: #E5E5E5;
            border-top-left-radius: 4px;
            border-top-right-radius: 4px;
            bottom: 0;
            right: 58px;
            padding: 0.6em 1.1em;
        }
    }
</style>