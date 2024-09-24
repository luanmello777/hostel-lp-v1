<template>
    <div class="bg-secondary pt-sm-16">
        <div class="d-md-flex pt-16 pb-16 px-2 mt-xl-16" align="center" justify="center" id="contato">

            <div class="w-100" align="center" justify="center">
                <v-form ref="form" action="https://formsubmit.co/soulhostelnatal@gmail.com" method="POST" @submit.prevent="validateForm">
                    <v-container class="mt-lg-16 pt-lg-16 mb-16 mb-md-0">
                      <v-row>
                        <v-col cols="12" sm="12" md="12" class="rounded-xl">
                          <v-text-field v-model="nome" name="nome" label="Nome" color="blue" hint="Informe seu Nome" required></v-text-field>
                        </v-col>
                
                        <v-col cols="12" sm="12" md="12">
                          <v-text-field v-model="email" name="email" label="E-mail" placeholder="email@email.com.br" hint="Informe seu E-mail" color="blue" required></v-text-field>
                        </v-col>
                
                        <v-col cols="12" sm="12" md="12">
                          <v-text-field v-model="whatsapp" name="whatsapp" label="WhatsApp" color="blue" placeholder="ddd + número" hint="Informe seu WhatsApp" required></v-text-field>
                        </v-col>
                
                        <v-col cols="12" sm="12" md="12">
                          <v-text-field v-model="mensagem" name="mensagem" label="Consultar Hospedagem" color="blue" hint="Informe sua Mensagem" required></v-text-field>
                        </v-col>
                      </v-row>
                
                      <input type="hidden" name="_next" value="https://www.booking.com/hotel/br/soul-hostel-natal.pt-br.html?label=gen173nr-1BCAEoggI46AdIM1gEaCCIAQGYAS24ARfIAQzYAQHoAQGIAgGoAgO4AuKh4bMGwAIB0gIkNjg1OTVkMjMtMDU1ZC00MTYzLWJkZGYtYWM4M2Y4ZTRjNTJm2AIF4AIB&sid=b7317855976ce3f9986bc94c9ec1d674&aid=304142&ucfs=1&arphpl=1&dest_id=5718445&dest_type=hotel&group_adults=2&req_adults=2&no_rooms=1&group_children=0&req_children=0&hpos=1&hapos=1&sr_order=popularity&srpvid=f38475b479800133&srepoch=1719161077&from_sustainable_property_sr=1&from=searchresults">
                      <input type="hidden" name="_captcha" value="false">
                      <input type="hidden" name="_subject" value="Novo envio de formulário!">
                
                      <div align="center">
                        <v-btn type="submit" class="bg-blue w-75 w-lg-50 mt-md-8 rounded-pill" size="large">
                          <h3 class="text-white">BOOKING.COM</h3>
                        </v-btn>
                      </div>
                    </v-container>
                  </v-form>
            </div>


            <div class="w-100">
                <h3
                    class="font text-terciary mt-4 text-sm-h3 text-md-h1 text-lg-h1 mt-sm-7 mt-md-16 pt-lg-16 d-lg-none">
                    Contato e
                    <br class="d-none d-lg-block d-lg-none">Reservas
                </h3>

                <h3 class="font text-terciary mt-5 pt-5 d-none d-lg-block"
                    style="font-size: 100px; line-height: 100px;">Contato e
                    <br>Reservas
                </h3>

                <div class="mt-3 mt-sm-5 mt-lg-16 w-100">
                    <v-btn class="bg-green rounded-pill w-75 w-sm-50 d-lg-none" href="https://api.whatsapp.com/send?phone=558499900268&text=Ol%C3%A1%21%20Estou%20vindo%20do%20Google%20e%20gostaria%20de%20valores%20e%20op%C3%A7%C3%B5es%20de%20reservas%21"
                        target="_blank">
                        <h4>Whatsapp</h4>
                    </v-btn>

                    <v-btn class="bg-green rounded-pill w-50 d-none d-lg-block" size="x-large" height="60"
                        href="https://api.whatsapp.com/send?phone=558499900268&text=Ol%C3%A1%21%20Estou%20vindo%20do%20Google%20e%20gostaria%20de%20valores%20e%20op%C3%A7%C3%B5es%20de%20reservas%21" target="_blank">
                        <h4 class="pt-5">Whatsapp</h4>
                    </v-btn>
                    <br>

                    <v-btn class="bg-pink rounded-pill my-3 w-75 w-sm-50 d-lg-none"
                        href="https://www.instagram.com/soulhostelnatal_/" target="_blank">
                        <h4>Instagram</h4>
                    </v-btn>

                    <v-btn class="bg-pink rounded-pill w-50 d-none d-lg-block" size="x-large" height="60"
                        href="https://www.instagram.com/soulhostelnatal_/" target="_blank">
                        <h4 class="pt-5">Instagram</h4>
                    </v-btn>
                    <br>

                    <v-btn class="bg-black rounded-pill w-75 w-sm-50 d-lg-none"
                        href="mailto:soulhostelnatal@gmail.com" target="_blank">
                        <h4>E-mail</h4>
                    </v-btn>

                    <v-btn class="bg-black rounded-pill w-50 d-none d-lg-block" size="x-large" height="60"
                        href="mailto:soulhostelnatal@gmail.com" target="_blank">
                        <h4 class="pt-5">E-mail</h4>
                    </v-btn>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.font {
    font-family: "Berkshire Swash", serif;
}
</style>

<script setup>
import { ref } from 'vue';

const nome = ref('');
const email = ref('');
const whatsapp = ref('');
const mensagem = ref('');

const form = ref(null);

const validateForm = () => {
  if (!nome.value || !email.value || !whatsapp.value || !mensagem.value) {
    alert('Por favor, preencha todos os campos antes de enviar.');
  } else {
    form.value.submit();
  }
};
</script>