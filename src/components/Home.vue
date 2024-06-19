<template>
  <div>
    <v-img src="/fundopraia.jpg">

      <div class="pt-14 ml-5 mt-10" style="line-height: 20px;">

        <h3 class="font text-white pl-1 font-weight-light"><span class="text-primary">FÉRIAS</span> EM</h3>
        <h1 class="font text-white font-weight-light"><svg-icon class="text-primary" type="mdi" :path="path" />NATAL-RN
        </h1>
        <h6 class="text-white font-weight-light pl-1" style="font-size: 5px; line-height: 16px; ">HOSPEDAGEM <span
            class="font-weight-bold text-primary">ACONCHEGANTE</span> COM VALORES <span
            class="font-weight-bold text-primary">PROMOCIONAIS</span></h6>

            <div>
              <v-btn class="bg-primary rounded-pill w-50" size="small">CONSULTAR RESERVAS</v-btn>
            </div>
      </div>




    </v-img>
  </div>

</template>

<style scoped>
.font {
  font-family: "Bree Serif", serif;
}
</style>

<script setup>
import { ref } from 'vue';
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiMapMarkerRadius } from '@mdi/js';

const path = ref(mdiMapMarkerRadius);
</script>