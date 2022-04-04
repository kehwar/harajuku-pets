<template>
    <v-app>
        <v-app-bar app class="app-bar">
            <HarajukuLogo v-if="true" class="app-bar-logo"></HarajukuLogo>
            <v-toolbar-title>Harajuku Pets</v-toolbar-title>
        </v-app-bar>
        <v-main>
            <v-container>
                <Nuxt />
            </v-container>
        </v-main>
        <v-footer app>
            <span>&copy; {{ new Date().getFullYear() }}</span>
        </v-footer>
    </v-app>
</template>

<script>
import HarajukuLogo from '~/components/harajukuLogo.vue'

export default {
    name: 'DefaultLayout',
    components: { HarajukuLogo },
}
</script>

<style scoped>
.app-bar {
    display: flex;
    gap: 10px;
    justify-content: center;
}

.app-bar-logo {
    position: absolute;
    right: calc(100%);
}
</style>
