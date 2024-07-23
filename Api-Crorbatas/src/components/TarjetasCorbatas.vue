<script setup>
import { ref } from 'vue';

defineProps({
  items: Array,
})

const indexAmpliado = ref(null) // Variable reactiva para guardar el índice de la imagen ampliada


function toggleAmpliacion(index) { // Función para ampliar la imagen
  indexAmpliado.value = indexAmpliado.value === index ? null : index // Si el índice es el mismo, lo pone a null, si no, lo pone al índice  
}
</script>

<template>
  <div class="container">
    <div v-for="item in items" :key="item.id"class="tarjeta" 
    >
      <div class="img">
        <img :src="item.foto" alt="Foto de corbata" @click="toggleAmpliacion(item.id)" :class="{ ampliada: indexAmpliado === item.id }" /> <!--  Añade la clase ampliada si el índice es el mismo -->
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
  margin-top: 13px;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  opacity: 0.9;
}

.tarjeta {
  width: 80%;
  transition: transform 0.5s ease;
  cursor: pointer;
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
  transition: transform 0.5s ease; /* Añade transición suave */
}

img.ampliada {
  transform: scale(3); 
}

.texto {
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