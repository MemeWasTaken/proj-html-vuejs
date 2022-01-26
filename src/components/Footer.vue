<template>
    <footer id="ftr">
        <UpperFooter 
            :foot="foo"
        />
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
        },
        data () { return { "foo": this.foot, } },
        props: [ 'foot' ],
    }
</script>

<style lang="scss" scoped>

</style>