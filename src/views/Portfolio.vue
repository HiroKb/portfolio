<template>
    <v-container class="d-flex flex-column align-center">
        <div class="portfolio">

            <div class="portfolio__item d-flex flex-column align-center">
                <section-title>ShareCalendar</section-title>
                <v-row class="mt-4" style="width: 100%">
                    <v-col cols="6" class="elevation-2">
                        <v-img src="../assets/share_calendar.png"></v-img>
                    </v-col>
                    <v-col cols="6" class="d-flex justify-center align-center">
                        <div class="d-flex flex-column align-center">
                            <h3>シンプルなスケジュール共有SPAです</h3>
                            <div class="mt-4">
                                <skill-chip color="#41B882">Vue.js</skill-chip>
                                <skill-chip color="#F72C21" class="ml-2">Laravel</skill-chip>
                                <skill-chip color="#252F3E" class="ml-2">AWS</skill-chip>
                            </div>
                            <p class="font-weight-bold mt-4 mb-2">Link: <a href="https://share-calendar.link">ShareCalendar</a></p>
                            <p class="font-weight-bold">Code/Infra: <a href="https://github.com/HiroKb/ShareCalendar">GitHub</a></p>
                        </div>
                    </v-col>
                </v-row>
            </div>

            <div class="portfolio__item d-flex flex-column align-center">
                <section-title>Portfolio</section-title>
                <v-row class="mt-4" style="width: 100%">
                    <v-col cols="6" class="d-flex justify-center align-center">
                        <div class="d-flex flex-column align-center">
                            <h3>当ポートフォリオです</h3>
                            <div class="mt-4">
                                <skill-chip color="#41B882">Vue.js</skill-chip>
                            </div>
                            <p class="font-weight-bold mt-4">Code: <a href="https://github.com/HiroKb/portfolio">GitHub</a></p>
                        </div>
                    </v-col>
                    <v-col cols="6" class="elevation-2">
                        <v-img src="../assets/portfolio.png"></v-img>
                    </v-col>
                </v-row>
            </div>
        </div>
    </v-container>
</template>

<script>
    import SectionTitle from "../components/SectionTitle";
    import SkillChip from "../components/SkillChip";
    export default {
        name: "Portfolio",
        components: {SectionTitle,SkillChip}
    }
</script>

<style scoped>
    .portfolio{
        margin-top: 160px;
        width: 100%;
    }
    .portfolio__item:not(:first-of-type){
        margin-top: 120px;
    }
    .portfolio__item:last-of-type{
        margin-bottom: 120px;
    }
    h3{
        font-size: 18px;
        color: gray;
        opacity: .8;
    }
</style>
