<script setup>
import { ref } from 'vue'
import { items } from '@/corbatas/data'
import TarjetasCorbatas from '@/components/TarjetasCorbatas.vue'

</script>

<template>

<TarjetasCorbatas :items="items" />

</template>

<style scoped>
:root {
  height: 100%;
  width: 100%;
}


</style>
