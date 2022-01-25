<template>
    <main>
        <Jumbo />
        <SectionChallenge />
        <SectionTraining />
        <SectionSecondJumbo />
    </main>
</template>

<script>
    import Jumbo from './partials/main/Jumbo.vue'
    import SectionChallenge from './partials/main/SectionChallenge.vue'
    import SectionTraining from './partials/main/SectionTraining.vue'
    import SectionSecondJumbo from './partials/main/SectionSecondJumbo.vue'

    export default {
        name: "Main",
        components: {
            Jumbo,
            SectionChallenge,
            SectionTraining,
            SectionSecondJumbo,
        }
    }
</script>

<style lang="scss" scoped>

</style>