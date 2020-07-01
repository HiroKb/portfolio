<template>
    <v-container class="d-flex flex-column align-center">
        <div class="profile d-flex flex-column align-center">
            <p class="section-title mb-0">Profile</p>
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
            <p class="section-title mb-0">Skills</p>
            <div class="skill__section">
                <v-chip color="#F16528" class="skill__chip">HTML</v-chip>
                <v-chip color="#2C65F1" class="skill__chip">CSS</v-chip>
            </div>
            <div class="skill__section">
                <v-chip color="#F7DF1F" class="skill__chip">JavaScript</v-chip>
                <v-chip color="#21609B" class="skill__chip">jQuery</v-chip>
                <v-chip color="#41B882" class="skill__chip">Vue.js</v-chip>
            </div>
            <div class="skill__section">
                <v-chip color="#6181B6" class="skill__chip">PHP</v-chip>
                <v-chip color="#F72C21" class="skill__chip">Laravel</v-chip>
            </div>
        </div>
    </v-container>
</template>

<script>
    export default {
        name: 'About',
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
    .skill__chip{
        font-size: 16px;
        font-weight: bold;
        color: white;
    }
    .skill__chip:not(:first-child){
        margin-left: 8px;
    }
</style>
