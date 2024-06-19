<template>
  <v-app>
    <v-main>
      <Navbar />
      <Home />
      <Sobre />
      <Localizaçao />
      <Contato />
      <Footer />
    </v-main>
  </v-app>
</template>

<script setup>
import Home from '@/components/Home.vue'
import Navbar from '@/components/Navbar.vue'
import Sobre from '@/components/Sobre.vue'
import Localizaçao from '@/components/Localizaçao.vue'
import Contato from '@/components/Contato.vue'
import Footer from '@/components/Footer.vue'
</script>