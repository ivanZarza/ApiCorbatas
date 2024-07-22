<script setup>

defineProps(['items'])

</script>

<template>
  <div class="container">
    <div class="tarjeta" v-for="item in items" :key="item.id">
      <img :src="item.foto" alt="imagen de corbata" />
      <h1>{{ item.nombre }}</h1>
      <p>{{ item.descripcion }}</p>
    </div>
  </div>
</template>

<style scoped>
.container {
  width: 80;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  opacity: 0.8;

}
.tarjeta {
  width: 80%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
  gap: 20px;
  padding: 20px;
  color: black;
  background-color: rgb(194, 194, 194);
}

img {
  width: 80px;
}
</style>