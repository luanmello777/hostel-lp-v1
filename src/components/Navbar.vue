<template>
    <v-app-bar align="center" justify="center" class="bg-quartiary" height="80">
        <v-btn icon="mdi-menu" size="x-large"></v-btn>

        <v-app-bar-title class="mr-3"><v-img src="/logo.jpg" height="70" class="w-100" /></v-app-bar-title>

        <v-btn icon="mdi-instagram" size="x-large" href="https://www.instagram.com/soulhostelnatal_/" target="_blank" />

    </v-app-bar>
</template>

<script setup>
import { useDisplay } from 'vuetify';

const { smAndDown } = useDisplay()
</script>