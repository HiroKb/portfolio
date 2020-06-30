<template>
    <v-app>
        <v-app-bar
            app
            color="primary"
            dark
        >
            <router-link to="/" class="white--text">Top</router-link>
            <router-link to="/about" class="white--text">About</router-link>
            <router-link to="/portfolio" class="white--text">Portfolio</router-link>
            <router-link to="/contact" class="white--text">Contact</router-link>
        </v-app-bar>
        <v-content>
            <router-view/>
        </v-content>
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
