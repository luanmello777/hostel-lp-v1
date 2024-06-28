<template>
    <v-app-bar align="center" justify="center" class="bg-quartiary" height="80">
        <v-menu>
            <template v-slot:activator="{ props }">
                <v-btn icon="mdi-menu" size="x-large" v-bind="props"></v-btn>
            </template>
            <v-list>
                <v-list-item class="text-terciary" :href="item.click" @click="redirecionarPara(item)"
                    v-for="(item, index) in itemsMenu" :key="index" :value="index">
                    <v-list-item-title>{{ item.title }}</v-list-item-title>
                </v-list-item>
            </v-list>
        </v-menu>

        <v-app-bar-title class="mr-3"><v-img src="/logo.jpg" height="70" class="w-100" /></v-app-bar-title>

        <v-btn icon="mdi-instagram" size="x-large" href="https://www.instagram.com/soulhostelnatal_/" target="_blank" />

    </v-app-bar>
</template>

<script setup>
const itemsMenu = [
    { title: 'O Hostel', click: '#hostel' },
    { title: 'Sobre', click: '#sobre' },
    { title: 'Localização', click: '#localizaçao' }, 
    { title: 'Contato', click: '#contato' }
]
</script>
