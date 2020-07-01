<template>
    <v-container class="d-flex flex-column align-center">
        <div class="profile d-flex flex-column align-center">
            <section-title class="mb-0">Profile</section-title>
            <v-img
                    alt="プロフィールイメージ"
                    src="../assets/icon.jpg"
                    class="icon"
                    style="border-radius: 50%"
                    height="160"
                    width="160"
                    aspect-ratio="1"
            ></v-img>
            <p class="text-center profile__text my-2">建設業・農業・飲食業等を経験後、<br>家業である不動産業に従事しています。</p>
            <p class="profile__text">独学でプログラミング学習中です。</p>
        </div>
        <div class="skill d-flex flex-column align-center mt-6">
            <section-title class="mb-0">Skills</section-title>
            <div class="skill__section">
                <skill-chip color="#F16528">HTML</skill-chip>
                <skill-chip color="#2C65F1" class="ml-2">CSS</skill-chip>
            </div>
            <div class="skill__section">
                <skill-chip color="#F7DF1F">JavaScript</skill-chip>
                <skill-chip color="#21609B" class="ml-2">jQuery</skill-chip>
                <skill-chip color="#41B882" class="ml-2">Vue.js</skill-chip>
            </div>
            <div class="skill__section">
                <skill-chip color="#6181B6">PHP</skill-chip>
                <skill-chip color="#F72C21" class="ml-2">Laravel</skill-chip>
            </div>
        </div>
    </v-container>
</template>

<script>
    import SkillChip from "../components/SkillChip";
    import SectionTitle from "../components/SectionTitle";
    export default {
        name: 'About',
        components:{SkillChip, SectionTitle}
    }
</script>

<style scoped>
    .profile{
        margin-top: 160px;
    }
    .profile__text{
        font-size: 18px;
    }
    .skill__section:not(:first-of-type){
        margin-top: 8px;
    }
</style>
