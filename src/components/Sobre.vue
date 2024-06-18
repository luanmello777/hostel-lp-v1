<template>
    <div align="center" justify="center">
        <div class="bg-secondary pt-16 pb-16">
            <h1 class="font text-terciary">Soul Hostel</h1>
            <h6 class="text-terciary font-weight-light">Não é apenas uma hospedagem.</h6>
            <h6 class="text-terciary font-weight-light">Somos <span class="text-black font-weight-bold">o seu lar longe
                    de
                    casa!</span></h6>


            <v-container class="d-flex mt-10" align="center" justify="center">
                <v-carousel :show-arrows="false" cycle hide-delimiters height="300" class="rounded-lg">
                    <v-carousel-item cover v-for="(blocoOne, i) in blocoOne" :key="i" :src="blocoOne.src"></v-carousel-item>
                </v-carousel>

                <v-carousel :show-arrows="false" cycle hide-delimiters height="300" class="rounded-lg ml-2 mr-sm-2">
                    <v-carousel-item cover v-for="(blocoTwo, i) in blocoTwo" :key="i" :src="blocoTwo.src"></v-carousel-item>
                </v-carousel>

                <v-carousel :show-arrows="false" cycle hide-delimiters height="300"
                    class="d-none d-sm-block rounded-lg">
                    <v-carousel-item cover v-for="(blocoThree, i) in blocoThree" :key="i" :src="blocoThree.src"></v-carousel-item>
                </v-carousel>
            </v-container>



            <v-row class="w-100 mt-16">
                <v-col cols="12" lg="4">
                    <div class="bg-white rounded-lg py-3 px-3" align="left">
                        <v-avatar image="/iconpraia.jpg" size="50" />
                        <h2 class="mt-3 font-weight-bold">Praias</h2>
                        <p>Estamos localizados apenas<br><span class="font-weight-bold">100m</span> da praia de <span class="font-weight-bold">Ponta Negra</span>.</p>
        

                        <div>
                            <v-btn class="bg-primary mt-6 rounded-pill">Saiba Mais</v-btn>
                        </div>
                    </div>

                </v-col>

                <v-col cols="12" lg="4">
                    <div class="bg-white rounded-lg py-3 px-3" align="left">
                        <v-avatar image="/iconsuite.jpg" size="50" />
                        <h2 class="mt-3 font-weight-bold">Acomodações</h2>
                        <p>Diversas opções de hospedagem para todas as necessidades.<br> Quartos com <span class="font-weight-bold">ventilador</span> ou <br><span class="font-weight-bold">ar-condicionado</span>.</p>


                        <div class="d-flex">
                            <v-btn class="bg-primary mt-6 rounded-pill">Saiba Mais</v-btn>
                            <v-btn class="bg-primary mt-6 rounded-pill ml-5">Consultar</v-btn>
                        </div>

                    </div>

                </v-col>

                <v-col cols="12" lg="4">
                    <div class="bg-white rounded-lg py-3 px-3" align="left">
                        <v-avatar image="/iconexpe.jpg" size="50" />
                        <h2 class="mt-3 font-weight-bold">Experiências</h2>
                        <p>Um <span class="font-weight-bold">ambiente acolhedor</span> com experiências únicas e uma conexão autêntica.</p>


                        <div>
                            <v-btn class="bg-primary mt-6 rounded-pill">Saiba Mais</v-btn>
                        </div>

                    </div>

                </v-col>
            </v-row>
        </div>

        <div>
            <br>
            <br>
            <br>
            <br>
        </div>
    </div>










</template>

<style scoped>
.font {
    font-family: "Berkshire Swash", serif;
}
</style>

<script setup>
import { ref } from 'vue'

const blocoOne = ref([
    {
        src: 'foto1bloco1.jpg',
    },
    {
        src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
    },
    {
        src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
    },
    {
        src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
    },
])

const blocoTwo = ref([
    {
        src: 'foto1bloco2.jpg',
    },
    {
        src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
    },
    {
        src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
    },
    {
        src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
    },
])

const blocoThree = ref([
    {
        src: 'foto1bloco3.jpg',
    },
    {
        src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
    },
    {
        src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
    },
    {
        src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
    },
])
</script>