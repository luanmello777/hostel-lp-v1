<template>
    <div align="center" justify="center">
        <div class="bg-secondary pt-16 pb-16">
            <h1 class="font text-terciary mt-sm-16 pt-lg-16 text-sm-h1 d-xl-none">Soul Hostel</h1>
            <h1 class="font text-terciary d-none d-xl-block mt-16 pt-16" style="font-size: 150px">Soul Hostel</h1>

            <h6 class="text-terciary font-weight-light mt-sm-5 text-sm-h5 text-xl-h4">Não é apenas uma hospedagem.</h6>
            <h6 class="text-terciary font-weight-light text-sm-h5 text-xl-h4 pb-xl-16">Somos <span
                    class="text-terciary font-weight-bold">o
                    seu lar longe
                    de
                    casa!</span></h6>


            <div class="d-flex mt-10 mt-sm-16 pt-sm-16 px-3 pt-md-16 pb-xl-16" align="center" justify="center">
                <v-carousel :show-arrows="false" cycle hide-delimiters height="350"
                    class="rounded-lg mr-sm-2 carousel-xl">
                    <v-carousel-item cover v-for="(blocoOne, i) in blocoOne" :key="i"
                        :src="blocoOne.src"></v-carousel-item>
                </v-carousel>

                <v-carousel :show-arrows="false" cycle hide-delimiters height="350"
                    class="d-none d-sm-block rounded-lg ml-2 mr-md-2 carousel-xl">
                    <v-carousel-item cover v-for="(blocoTwo, i) in blocoTwo" :key="i"
                        :src="blocoTwo.src"></v-carousel-item>
                </v-carousel>

                <v-carousel :show-arrows="false" cycle hide-delimiters height="350"
                    class="d-none d-md-block rounded-lg ml-2 carousel-xl">
                    <v-carousel-item cover v-for="(blocoThree, i) in blocoThree" :key="i"
                        :src="blocoThree.src"></v-carousel-item>
                </v-carousel>
            </div>



            <v-row class="w-100 mt-16 mb-sm-16 pt-sm-16 pb-xl-16">
                <v-col cols="12" sm="6" md="4" lg="4">
                    <div class="bg-white rounded-lg py-5 px-3" align="left">
                        <v-avatar image="/iconpraia.jpg" size="50" class="d-lg-none" />
                        <v-avatar image="/iconpraia.jpg" size="100" class="d-none d-lg-block" />

                        <h2 class="mt-3 font-weight-bold text-md-h4 text-xl-h3">Praias</h2>
                        <p class="text-md-h6 text-xl-h4 mt-lg-5 font-weight-light">Estamos localizados apenas <br>
                            <span class="font-weight-bold">100m</span>
                            da praia de <span class="font-weight-bold">Ponta Negra</span>.
                        </p>


                        <div>
                            <v-btn class="bg-primary mt-6 rounded-pill d-lg-none">
                                <h4>Saiba Mais</h4>
                            </v-btn>
                            <v-btn class="bg-primary mt-6 rounded-pill d-none d-lg-block" size="x-large">
                                <h4>Saiba
                                    Mais</h4>
                            </v-btn>
                        </div>
                    </div>

                </v-col>

                <v-col cols="12" sm="6" md="4" lg="4">
                    <div class="bg-white rounded-lg py-5 px-3" align="left">
                        <v-avatar image="/iconsuite.jpg" size="50" class="d-lg-none" />
                        <v-avatar image="/iconsuite.jpg" size="100" class="d-none d-lg-block" />

                        <h2 class="mt-3 font-weight-bold text-md-h4 text-xl-h3">Acomodações</h2>
                        <p class="text-md-h6 text-xl-h4 mt-lg-5 font-weight-light">Diversas opções de hospedagem
                            <br>para <span class="font-weight-bold">todas as
                                necessidades</span>.
                        </p>


                        <div class="d-flex">
                            <v-btn class="bg-primary mt-6 rounded-pill  d-lg-none">
                                <h4>Saiba Mais</h4>
                            </v-btn>
                            <v-btn class="bg-primary mt-6 rounded-pill  d-none d-lg-block" size="x-large">
                                <h4>Saiba
                                    Mais</h4>
                            </v-btn>


                            <v-btn class="bg-primary mt-6 rounded-pill ml-5  d-lg-none"
                                href=" https://wa.me/558499900268" target="_blank"><h4>Consultar</h4></v-btn>

                            <v-btn class="bg-primary mt-6 rounded-pill ml-5 d-none d-lg-block" size="x-large"
                                href=" https://wa.me/558499900268" target="_blank">
                                <h4 class="pt-4">Consultar</h4>
                            </v-btn>
                        </div>

                    </div>

                </v-col>

                <v-col cols="12" sm="6" md="4" lg="4">
                    <div class="bg-white rounded-lg py-5 px-3" align="left">
                        <v-avatar image="/iconexpe.jpg" size="50" class="d-lg-none" />
                        <v-avatar image="/iconexpe.jpg" size="100" class="d-none d-lg-block" />


                        <h2 class="mt-3 font-weight-bold text-md-h4 text-xl-h3">Experiência</h2>
                        <p class="text-md-h6 text-xl-h4 mt-lg-5 font-weight-light">Um <span
                                class="font-weight-bold">ambiente
                                acolhedor</span> e uma
                            conexão autêntica.</p>


                        <div>
                            <v-btn class="bg-primary mt-6 rounded-pill d-lg-none"><h4>Saiba Mais</h4></v-btn>
                            <v-btn class="bg-primary mt-6 rounded-pill d-none d-lg-block" size="x-large"><h4>Saiba
                                Mais</h4></v-btn>
                        </div>

                    </div>
                </v-col>
            </v-row>
        </div>

        <div>
            <v-container align="center" justify="center" class="py-sm-16 my-md-8 my-lg-16">
                <div style="border: solid 4px #FCC009;" class="rounded-xl pt-5 py-md-16 my-10 w-sm-75 w-md-100 w-xl-75">
                    <h5 class="font-weight-light text-sm-h6 text-md-h4 text-xl-h3">O <span
                            class="font-weight-bold text-terciary">Soul
                            Hostel</span> é o
                        hostel mais bem avaliado<br>
                        de <span class="font-weight-bold text-terciary">Natal-RN</span> na Booking e no Google!</h5>


                    <div class="d-flex">
                        <v-img src="/booking.png" height="110" class="d-sm-none" />
                        <v-img src="/booking.png" height="160" class="d-none d-sm-block d-md-none" />
                        <v-img src="/booking.png" height="250" class="d-none d-md-block d-xl-none" />
                        <v-img src="/booking.png" height="350" class="d-none d-xl-block" />

                        <v-img src="/google.png" height="110" class="d-sm-none" />
                        <v-img src="/google.png" height="160" class="d-none d-sm-block d-md-none" />
                        <v-img src="/google.png" height="250" class="d-none d-md-block d-xl-none" />
                        <v-img src="/google.png" height="350" class="d-none d-xl-block" />
                    </div>
                </div>
            </v-container>
        </div>
    </div>
</template>

<style scoped>
.font {
    font-family: "Berkshire Swash", serif;
}

@media (min-width: 1500px) {
    .carousel-xl {
        height: 750px !important;
    }
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