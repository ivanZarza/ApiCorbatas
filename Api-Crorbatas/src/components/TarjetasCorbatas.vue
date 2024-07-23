<script setup>

defineProps(['items'])

</script>

<template>
  <div class="container">
    <div class="tarjeta" v-for="item in items" :key="item.id">
      <div class="img">
        <img :src="item.foto" alt="imagen de corbata" />
      </div>
      <div class="texto">
        <h1>{{ item.nombre }}</h1>
        <p>{{ item.descripcion }}</p>
      </div>
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
  opacity: 0.9;
}

.tarjeta {
  width: 80%;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-evenly;
  align-items: center;
  gap: 10px;
  padding: 20px;
  color: black;
  background-color: rgb(92, 92, 92);
}

.img {
  width: 15rem;
}

img {
  width: 15rem;
}

.texto{
  width: 50%;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  gap: 20px;
  padding: 20px;
  color: rgb(255, 255, 255);
  font-size: 1.1rem;

}
</style>