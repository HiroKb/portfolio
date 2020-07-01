<template>
    <v-app>
        <header class="header">
            <div class="d-flex container justify-space-between" >
                <router-link to="/" class="header__menu">Top</router-link>
                <div>
                    <router-link to="/portfolio" class="header__menu">Portfolio</router-link>
                    <router-link to="/about" class="header__menu">About</router-link>
                </div>
            </div>
        </header>
        <v-main>
            <transition mode="out-in">
                <router-view/>
            </transition>
        </v-main>
    </v-app>
</template>

<script>

export default {
    name: 'App',
    data: () => ({
        //
    }),
};
</script>

<style>
    .container{
        max-width: 1200px !important;
    }
    p{
        color: gray;
    }
</style>
<style scoped>
    .header{
        position: fixed;
        width: 100%;
        z-index: 1;
        background-color: rgba(255, 255, 255, .8);
    }
    .header__menu{
        position: relative;
        font-weight: bold;
        text-decoration: none;
        color: gray;
        font-size: 24px;
        opacity: .8;
    }
    .header__menu:after{
        content:"";
        display:block;
        width:100%;
        height:4px;
        background-color: gray;
        position:absolute;
        bottom: -2px;
        left:0;
        border-radius: 4px;
        opacity: 0;
        transition: opacity .5s;
    }
    .header__menu:not(:first-of-type){
        margin-left: 32px;
    }
    .router-link-exact-active::after{
        opacity: .8;
        transition: opacity .5s;
    }

    .v-enter {
        transform: translate(0, 100vh);
        opacity: 0;
    }
    .v-enter-to {
        transform: translate(0, 0);
        opacity: 1;
    }
    .v-enter-active {
        transition: all .5s ease-in-out 0s;
    }
    .v-leave {
        transform: translate(0, 0);
        opacity: 1;
    }
    .v-leave-to {
        transform: translate(0, -100vh);
        opacity: 0;
    }
    .v-leave-active {
        transition: all .4s ease-in-out 0s;
    }
</style>
