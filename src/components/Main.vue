<template>
    <main>
        <Jumbo />
        <SectionChallenge />
        <SectionTraining />
        <SectionSecondJumbo />
        <SectionServicesCards />
        <SectionLatestArticles />
        <SectionBanner />
    </main>
</template>

<script>
    import Jumbo from './partials/main/Jumbo.vue'
    import SectionChallenge from './partials/main/SectionChallenge.vue'
    import SectionTraining from './partials/main/SectionTraining.vue'
    import SectionSecondJumbo from './partials/main/SectionSecondJumbo.vue'
    import SectionServicesCards from './partials/main/SectionServicesCards.vue'
    import SectionLatestArticles from './partials/main/SectionLatestArticles.vue'
    import SectionBanner from './partials/main/SectionBanner.vue'

    export default {
        name: "Main",
        components: {
            Jumbo,
            SectionChallenge,
            SectionTraining,
            SectionSecondJumbo,
            SectionServicesCards,
            SectionLatestArticles,
            SectionBanner,
        }
    }
</script>

<style lang="scss" scoped>

</style>