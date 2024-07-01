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


            <div class="d-flex mt-10 mt-sm-16 pt-sm-16 px-3 pt-md-16" align="center" justify="center" id="hostel">
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



            <v-row class="w-100 mt-16 mb-sm-16 pt-sm-16 pt-lg-10 mb-lg-10" id="sobre">
                <v-col cols="12" sm="6" md="4" lg="4">
                    <div class="bg-white rounded-lg py-5 px-3" align="left">
                        <v-avatar image="/iconpraia.jpg" size="50" class="d-lg-none" />
                        <v-avatar image="/iconpraia.jpg" size="100" class="d-none d-lg-block" />

                        <h2 class="mt-3 font-weight-bold text-md-h4 text-xl-h3">Praias</h2>
                        <p class="text-md-h6 text-xl-h4 mt-lg-5 font-weight-light">Estamos localizados apenas <br>
                            <span class="font-weight-bold">100m</span>
                            da praia de <span class="font-weight-bold">Ponta Negra</span>.
                        </p>
                        <v-dialog max-width="500">
                            <template v-slot:activator="{ props: activatorProps }">
                                <v-btn class="bg-primary mt-6 rounded-pill d-lg-none" v-bind="activatorProps">
                                    <h4>Saiba Mais</h4>
                                </v-btn>
                                <v-btn class="bg-primary mt-6 rounded-pill d-none d-lg-block" size="x-large"
                                    v-bind="activatorProps">
                                    <h4>Saiba
                                        Mais</h4>
                                </v-btn>
                            </template>

                            <template v-slot:default="{ isActive }">
                                <v-card title="Praias">
                                    <v-card-text>
                                        <ul>
                                            <li>100m da <span class="font-weight-bold">Praia de Ponta Negra</span></li>
                                            <li>13,7 km da <span class="font-weight-bold">Praia da Redinha</span></li>
                                            <li>8,3 km da <span class="font-weight-bold">Praia de Miami</span></li>
                                            <li>12,3 km do <span class="font-weight-bold">Forte dos Reis Magos</span>
                                            </li>
                                            <li>6,8 km do <span class="font-weight-bold">Parque das Dunas</span></li>
                                            <li>10,2 km do <span class="font-weight-bold">Centro de Turismo de
                                                    Natal</span></li>
                                            <li>32 km do <span class="font-weight-bold">Maior Cajueiro do Mundo</span>
                                            </li>

                                        </ul>
                                    </v-card-text>

                                    <v-card-actions>
                                        <v-spacer></v-spacer>

                                        <v-btn text="Voltar" class="bg-primary rounded-pill"
                                            @click="isActive.value = false"></v-btn>
                                    </v-card-actions>
                                </v-card>
                            </template>
                        </v-dialog>
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
                            <v-dialog max-width="500">
                                <template v-slot:activator="{ props: activatorProps }">
                                    <v-btn class="bg-primary mt-6 rounded-pill  d-lg-none" v-bind="activatorProps">
                                        <h4>Saiba Mais</h4>
                                    </v-btn>
                                    <v-btn class="bg-primary mt-6 rounded-pill  d-none d-lg-block" size="x-large"
                                        v-bind="activatorProps">
                                        <h4>Saiba
                                            Mais</h4>
                                    </v-btn>
                                </template>

                                <template v-slot:default="{ isActive }">
                                    <v-card title="Acomodações">
                                        <v-card-text>
                                            <ul>
                                                <li><span class="font-weight-bold">Suite privativa para casais:</span>
                                                    Desfrute de
                                                    conforto e privacidade em nossa
                                                    suite especialmente decorada para casais, proporcionando um
                                                    ambiente romântico e acolhedor.</li>

                                                <br>

                                                <li><span class="font-weight-bold">Suite privativa para familia:</span>
                                                    Espaço
                                                    amplo e confortável, ideal para
                                                    famílias que desejam aproveitar momentos de lazer e descanso juntos,
                                                    com todas as comodidades necessárias para uma estadia agradável.
                                                </li>

                                                <br>

                                                <li>
                                                    <span class="font-weight-bold">Suite compartilhada:</span> Suite
                                                    compartilhada e econômica,
                                                    perfeita para mochileiros que procuram uma hospedagem prática e com
                                                    ambiente descontraído para conhecer outros viajantes.
                                                    (<span class="font-weight-bold">Suites separadas para Homens e
                                                        Mulheres</span>)
                                                </li>

                                                <br>

                                                <li>
                                                    <span class="font-weight-bold">Suite privativa:</span> Para os
                                                    viajantes/hóspedes solos que buscam tranquilidade e privacidade,
                                                    nossas
                                                    suites individuais são a escolha ideal, oferecendo um espaço
                                                    aconchegante e funcional.
                                                </li>
                                                <br>
                                                <p><span class="font-weight-bold">VENTILADOR</span> ou <span
                                                        class="font-weight-bold">AR-CONDICIONADO</span>.</p>



                                            </ul>
                                        </v-card-text>

                                        <v-card-actions>
                                            <v-spacer></v-spacer>

                                            <v-btn text="Voltar" class="bg-primary rounded-pill"
                                                @click="isActive.value = false"></v-btn>
                                        </v-card-actions>
                                    </v-card>
                                </template>
                            </v-dialog>


                            <v-btn class="bg-primary mt-6 rounded-pill ml-5  d-lg-none"
                                href=" https://wa.me/558499900268" target="_blank">
                                <h4>Consultar</h4>
                            </v-btn>

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
                                acolhedor</span> com uma
                            conexão autêntica.</p>

                        <v-dialog max-width="500">
                            <template v-slot:activator="{ props: activatorProps }">
                                <v-btn class="bg-primary mt-6 rounded-pill d-lg-none" v-bind="activatorProps">
                                    <h4>Saiba Mais</h4>
                                </v-btn>
                                <v-btn class="bg-primary mt-6 rounded-pill d-none d-lg-block" size="x-large"
                                    v-bind="activatorProps">
                                    <h4>Saiba
                                        Mais</h4>
                                </v-btn>
                            </template>

                            <template v-slot:default="{ isActive }">
                                <v-card title="Experiência">
                                    <v-card-text>
                                        <p>Desfrute do melhor que Natal tem a oferecer com a experiência de
                                            estar próximo a variedade de praias
                                            paradisíacas, perfeitas para relaxar, nadar e apreciar a vista. Além disso,
                                            a região é repleta de restaurantes que oferecem uma rica gastronomia local,
                                            proporcionando uma verdadeira imersão na cultura potiguar.</p>
                                    </v-card-text>

                                    <v-card-actions>
                                        <v-spacer></v-spacer>

                                        <v-btn text="Voltar" class="bg-primary rounded-pill"
                                            @click="isActive.value = false"></v-btn>
                                    </v-card-actions>
                                </v-card>
                            </template>
                        </v-dialog>
                    </div>
                </v-col>
            </v-row>
        </div>

        <div>
            <v-container align="center" justify="center" class="py-sm-16 my-md-8 my-lg-16">
                <div style="border: solid 4px #FCC009;" class="rounded-xl pt-5 py-md-16 my-10 w-sm-75 w-md-100 w-lg-75">
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
                        <v-img src="/google.png" height="250" class="d-none d-md-block d-lg-none" />
                        <v-img src="/google.png" height="260" class="d-none d-lg-block" />
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
        height: 600px !important;
    }
}

#sobre {
    scroll-margin-top: 100px;
}

#hostel {
    scroll-margin-top: 300px;
}
</style>

<script setup>
import { ref } from 'vue'

const blocoOne = ref([
    {
        src: 'soul.jpg',
    },
    {
        src: 'sala.jpg',
    },
    {
        src: 'localização.jpg',
    },
    {
        src: 'varanda.jpg',
    },
])

const blocoTwo = ref([
    {
        src: 'quarto1.jpg',
    },
    {
        src: 'quarto2.jpg',
    },
    {
        src: 'quarto3.jpeg',
    },
    {
        src: 'quarto4.jpg',
    },
])

const blocoThree = ref([
    {
        src: 'sala.jpg',
    },
    {
        src: 'varanda.jpg',
    },
    {
        src: 'escada.jpg',
    },
    {
        src: 'corredor.jpg',
    },
    {
        src: 'cozinha.jpg',
    },
])
</script>