<script setup>
import { items } from '@/corbatas/data'
import TarjetasCorbatas from './componentes/TarjetasCorbatas.vue';
import CabezeraPagina from '@/componentes/CabezeraPagina.vue';
import PiePagina from '@/componentes/PiePagina.vue';

</script>

<template>

  <CabezeraPagina />

  <TarjetasCorbatas class="corbatas" :items="items"/>

  <PiePagina />

</template>

<style scoped>
:root {
  height: 100%;
  width: 100%;
}


</style>
