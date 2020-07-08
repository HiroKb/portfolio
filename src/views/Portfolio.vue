<template>
    <v-container class="d-flex flex-column align-center">
        <div class="portfolio">

            <div class="portfolio__item d-flex flex-column align-center">
                <section-title>ShareCalendar</section-title>
                <v-row class="mt-sm-4 mt-2" style="width: 100%">
                    <v-col cols="sm-6 12" class="elevation-2">
                        <v-img src="../assets/share_calendar.png"></v-img>
                    </v-col>
                    <v-col cols="sm-6 12" class="d-flex justify-center align-center">
                        <div class="d-flex flex-column align-center">
                            <h3>シンプルなスケジュール共有SPA</h3>
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
                <v-row class="mt-sm-4 mt-2" style="width: 100%">
                    <v-col cols="sm-6 12" order-sm="2" class="elevation-2">
                        <v-img src="../assets/portfolio.png"></v-img>
                    </v-col>
                    <v-col cols="sm-6 12" order-sm="1" class="d-flex justify-center align-center">
                        <div class="d-flex flex-column align-center">
                            <h3>当ポートフォリオ</h3>
                            <div class="mt-4">
                                <skill-chip color="#41B882">Vue.js</skill-chip>
                                <skill-chip color="#7BC5FF" class="ml-2">Vuetify</skill-chip>
                            </div>
                            <p class="font-weight-bold mt-4">Code: <a href="https://github.com/HiroKb/portfolio">GitHub</a></p>
                        </div>
                    </v-col>
                </v-row>
            </div>

            <div class="portfolio__item d-flex flex-column align-center">
                <section-title>CafePage</section-title>
                <v-row class="mt-sm-4 mt-2" style="width: 100%">
                    <v-col cols="sm-6 12" class="elevation-2">
                        <v-img src="../assets/k's_cafe.jpg"></v-img>
                    </v-col>
                    <v-col cols="sm-6 12" class="d-flex justify-center align-center">
                        <div class="d-flex flex-column align-center">
                            <h3>架空のカフェホームページ</h3>
                            <div class="mt-4">
                                <skill-chip color="#CF649A">Sass</skill-chip>
                                <skill-chip color="#21609B" class="ml-2">jQuery</skill-chip>
                                <skill-chip color="#D34A47" class="ml-2">gulp</skill-chip>
                            </div>
                            <p class="font-weight-bold mt-4 mb-2">Link: <a href="https://sample1.hirokb.com">CafePage</a></p>
                            <p class="font-weight-bold">Code: <a href="https://github.com/HiroKb/fictional-cafe">GitHub</a></p>
                        </div>
                    </v-col>
                </v-row>
            </div>

            <div class="portfolio__item d-flex flex-column align-center">
                <section-title>OrgTas</section-title>
                <v-row class="mt-sm-4 mt-2" style="width: 100%">
                    <v-col cols="sm-6 12" order-sm="2" class="elevation-2">
                        <v-img src="../assets/orgtas.png"></v-img>
                    </v-col>
                    <v-col cols="sm-6 12" order-sm="1" class="d-flex justify-center align-center">
                        <div class="d-flex flex-column align-center">
                            <h3>タスク共有アプリ</h3>
                            <div class="mt-4">
                                <skill-chip color="#6181B6">PHP</skill-chip>
                                <skill-chip color="#21609B" class="ml-2">jQuery</skill-chip>
                            </div>
                            <p class="font-weight-bold mt-4 mb-2">Link: 未デプロイ</p>
                            <p class="font-weight-bold">Code: <a href="https://github.com/HiroKb/orgtas">GitHub</a></p>
                        </div>
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
        components: {SectionTitle,SkillChip},
        mounted() {
            scrollTo(0, 0)
        }
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

    @media screen and (max-width: 599px){
        .portfolio{
            margin-top: 80px;
        }
    }
</style>
