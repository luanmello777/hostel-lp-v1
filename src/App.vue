<template>
  <v-app>
    <v-main>
      <Navbar />
      <Home />
      <Sobre />
    </v-main>
  </v-app>
</template>

<script setup>
import Home from '@/components/Home.vue'
import Navbar from '@/components/Navbar.vue'
import Sobre from '@/components/Sobre.vue'
</script>
