<script setup>
import { items } from '@/corbatas/data'
import TarjetasCorbatas from '@/components/TarjetasCorbatas.vue'
import CabezeraPagina from './components/CabezeraPagina.vue';

</script>

<template>

  <CabezeraPagina />

  <TarjetasCorbatas class="corbatas" :items="items" />

</template>

<style scoped>
:root {
  height: 100%;
  width: 100%;
}


</style>
