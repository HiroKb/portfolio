<template>
    <v-chip :color="color" class="chip"><slot></slot></v-chip>
</template>

<script>
    export default {
        name: "SkillChip",
        props:{
            color: {
                type: String,
                required: true,
                default: ''
            },
        }
    }
</script>

<style scoped>
    .chip{
        font-size: 16px !important;
        font-weight: bold;
        color: white !important;
    }
</style>