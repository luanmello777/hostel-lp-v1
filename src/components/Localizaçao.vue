<template>
    <div class="bg-secondary pt-sm-16">
        <div class="d-flex pt-16 pb-16 px-2 px-sm-4 px-lg-10 mt-sm-4 mt-xl-16" align="center" justify="center" id="localizaçao">

            <div class="w-100 pt-sm-1 pl-xl-16 ml-lg-4 ml-md-8" align="left">
                <h2 class="font text-terciary text-sm-h3 text-md-h2 mt-md-16 d-lg-none">Localização</h2>
                <h2 class="font text-terciary d-none d-lg-block" style="font-size: 100px;">Localização</h2>

                <h6 class="font-weight-light pr-6 pr-sm-8 pr-md-10 pr-lg-16 text-sm-h6 mt-sm-1 mt-md-10 mt-lg-0 text-md-h5 text-lg-h4"
                    align="left" style="font-size: 9px;">
                    O <span class="text-terciary font-weight-bold">Soul Hostel</span> possui uma localização excepcional
                    que encanta os hóspedes. Situado a poucos
                    passos da <span class="text-terciary font-weight-bold">Praia de Ponta Negra</span>, oferece fácil acesso às águas do
                    mar. A proximidade conta com uma variedade de restaurantes, bares e lojas que proporcionam uma experiência
                    gastronômica e cultural.</h6>

                <h1 class="font-weight-light text-terciary pr-16 d-none d-xl-block"
                    align="left" style="line-height: 65px; font-size: 45px;">
                    O <span class="text-terciary font-weight-bold">Soul Hostel</span> possui uma localização excepcional
                    que encanta os hóspedes. <br class="d-none d-xl-block">Situado a poucos
                    passos da <span class="text-terciary font-weight-bold">Praia de Ponta Negra</span>, oferece fácil acesso às águas do
                    mar. A proximidade conta com uma variedade de restaurantes, bares e lojas que proporcionam uma experiência
                    gastronômica e cultural.</h1>


                <div class="mt-xl-16">
                    <v-btn class="bg-primary mt-3 rounded-pill w-75 mt-md-8 mt-xl-16 d-lg-none"
                        href="https://maps.app.goo.gl/kN7LXAo414Fpgem6A" target="_blank">
                        <h4>MAPA</h4>
                    </v-btn>

                    <v-btn class="bg-primary mt-6 rounded-pill d-none d-lg-block w-50" size="x-large"
                        href="https://maps.app.goo.gl/kN7LXAo414Fpgem6A" target="_blank">
                        <h4 class="pt-4">VER NO MAPA</h4>
                    </v-btn>
                </div>
            </div>

            <div class="w-100">
                <v-img src="/localização.jpg" cover height="210" class="rounded-lg d-sm-none" />
                <v-img src="/localização.jpg" cover height="400" class="rounded-lg d-none d-sm-block d-md-none" />
                <v-img src="/localização.jpg" cover height="600"
                    class="rounded-lg  d-none d-sm-none d-md-block d-xl-none" />
                <v-img src="/localização.jpg" cover height="850" class="rounded-lg w-75 d-none d-xl-block" />
            </div>
        </div>
    </div>

</template>

<style scoped>
.font {
    font-family: "Berkshire Swash", serif;
}

#localizaçao {
    scroll-margin-top: 40px;
}
</style>