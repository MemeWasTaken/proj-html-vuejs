<template>
    <main>
        <Jumbo />
        <SectionChallenge />
        <SectionTraining />
    </main>
</template>

<script>
    import Jumbo from './partials/main/Jumbo.vue'
    import SectionChallenge from './partials/main/SectionChallenge.vue'
    import SectionTraining from './partials/main/SectionTraining.vue'

    export default {
        name: "Main",
        components: {
            Jumbo,
            SectionChallenge,
            SectionTraining,
        }
    }
</script>

<style lang="scss" scoped>

</style>