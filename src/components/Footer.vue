<template>
    <footer>
        <UpperFooter />
        <BottomFooter />
    </footer>
</template>

<script>
    import UpperFooter from './partials/footer/UpperFooter.vue'
    import BottomFooter from './partials/footer/BotttomFooter.vue'

    export default {
        name: "Footer",
        components: {
            UpperFooter,
            BottomFooter,
        }
    }
</script>

<style lang="scss" scoped>

</style>