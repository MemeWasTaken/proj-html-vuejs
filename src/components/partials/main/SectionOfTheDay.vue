<template>
    <section class="of-the-day d-flex flex-column justify-content-center align-items-center">
    
        <div class="play-button rounded-circle">
            <i class="fas fa-play"></i>
        </div>
        <h1 class="pt-4">Crossfit workout of the day</h1>
        <h2 class="pt-3">November 15th, 2019</h2>
        <a class="text-decoration-none pt-2" href="">View all videos &rarr;</a>
            
    </section>
</template>

<script>
    export default {
        name: "SectionOfTheDay",
    }
</script>

<style lang="scss" scoped>
    @import '../../../assets/scss/partials/_variables.scss';

    .of-the-day {
        background-color: rgba(255, 255, 255, 0);
        background-image: linear-gradient(151deg, #4154ff 35%,#ff414b 100%), url('../../../assets/img/banner14-2x.jpg');
        background-blend-mode: multiply;
        background-size: cover;
        background-position: center;
        width: 100%;
        height: 640px;

        .play-button {
            background-color: #FFFFFF;
            color: $dodgerBlue;
            text-align: center;
            width: 6em;
            line-height: 6em;
            height: 6em;

            .fas.fa-play { font-size: 1.2em; }
        }
        h1 {
            color: #ffffff;
            font-size: 3.8em;
        }
        h2 {
            color: #FFF941;
            font-size: 2em;
        }
        a {
            color: #ffffff;
            font-size: 1.2em;
            font-weight: 500;
        }
    }
</style>