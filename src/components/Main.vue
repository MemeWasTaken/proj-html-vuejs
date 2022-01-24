<template>
    <main>
        <Jumbo />
        <SectionChallenge />
    </main>
</template>

<script>
    import Jumbo from './partials/main/Jumbo.vue'
    import SectionChallenge from './partials/main/SectionChallenge.vue'

    export default {
        name: "Main",
        components: {
            Jumbo,
            SectionChallenge,
        }
    }
</script>

<style lang="scss" scoped>

</style>