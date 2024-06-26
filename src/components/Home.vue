<template>
  <div>
    <v-img src="/fundopraia.jpg">

      <div class="background w-50 h-100 pl-2" style="line-height: 20px;" justify="center" align="left">

     
          <h4 class="font text-white font-weight-light pt-16" align="left">
            <span class="text-primary">FÉRIAS</span> EM
          </h4>

          <h1 class="font text-white font-weight-light">NATAL-RN
          </h1>

          <h6 class="text-white font-weight-light" style="font-size: 5px; line-height: 20px;">HOSPEDAGEM
            <span class="font-weight-bold text-primary">ACONCHEGANTE</span> COM VALORES <span
              class="font-weight-bold text-primary">PROMOCIONAIS</span>
          </h6>


          <div>
            <v-btn class="bg-primary rounded-pill w-50 mt-1 mt-sm-2 d-md-none" size="small">RESERVAS</v-btn>
          </div>



      </div>




    </v-img>
  </div>

</template>

<style scoped>
.font {
  font-family: "Bree Serif", serif;
}

.background {
  background-color: rgba(0, 0, 0, 0.685);
}
</style>

<script setup>
import { ref } from 'vue';
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiMapMarkerRadius } from '@mdi/js';

const path = ref(mdiMapMarkerRadius);
</script>