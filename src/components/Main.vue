<template>
    <main>
        <Jumbo />
        <SectionChallenge
            :chall="chal"
        />
        <SectionTraining 
            :train="trai"
        />
        <SectionSecondJumbo />
        <SectionServicesCards 
            :serv="ser"
        />
        <SectionLatestArticles 
            :latarts="larts"
        />
        <SectionBanner />
        <SectionPartners 
            :parts="pars"
        />
        <SectionOfTheDay />
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
    import SectionPartners from './partials/main/SectionPartners.vue'
    import SectionOfTheDay from './partials/main/SectionOfTheDay.vue'

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
            SectionPartners,
            SectionOfTheDay,
        },
        data() { 
            return { 
                "chal": this.chall, 
                "trai": this.train, 
                "ser": this.serv,
                "larts": this.latarts,
                "pars": this.parts,
            } 
        },
        props: [ 
            'chall',
            'train',
            'serv',
            'latarts',
            'parts',
        ],

    }
</script>

<style lang="scss" scoped>

</style>