<template>
    <h2 class="section-title"><slot></slot></h2>
</template>

<script>
    export default {
        name: "SectionTitle"
    }
</script>

<style scoped>
    .section-title{
        font-weight: bold;
        font-size: 24px;
        color: gray;
        opacity: .8;
    }
</style>