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
    <div v-for="item in items" :key="item.id" class="tarjeta">
      <div class="img">
        <img :src="item.foto" alt="Foto de corbata" @click="toggleAmpliacion(item.id)"
          :class="{ ampliada: indexAmpliado === item.id }" /> <!--  Añade la clase ampliada si el índice es el mismo -->
      </div>
      <div class="texto">
        <h1>{{ item.nombre }}</h1>
        <p>{{ item.descripcion }}</p>
        <p>{{ item.precio }}</p>
      </div>
    </div>
    <div class="pañuelo">
      <p>Todas las corbatas podran llevar pañuelo a juego bajo previo encargo</p>
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
  justify-content: center;
  gap: 20px;
  opacity: 0.95;
}

.tarjeta {
  width: 60%;
  transition: transform 0.5s ease;
  cursor: pointer;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-evenly;
  align-items: center;
  gap: 10px;
  padding: 10px;
  color: black;
  background-color: rgb(26, 26, 26);
  box-shadow: 10 10 3px rgba(170, 170, 170, 0.5);
}

.img {
  width: 40%;
}

img {
  width: 10rem;
  transition: transform 0.5s ease;
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

@media (max-width: 900px) {

  .container {
    width: 100%;
  }

  .tarjeta {
    width: 50%;
    text-align: center;
    font-size: 0.5rem;
  }
}

@media (max-width: 750px) {

  img {
    max-width: 100%;
  }

  .tarjeta {
    width: 80%;
    text-align: center;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    padding: 10px;
    gap: 10px;
  }

  .texto {
    max-width: 50%;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    gap: 10px;
    padding: 9px;
    color: rgb(255, 255, 255);
    font-size: 0.9rem;
    margin: none;
  }
}

.pañuelo {
  width: 60%;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  gap: 20px;
  padding: 20px;
  color: rgb(255, 255, 255);
  font-size: 1.1rem;
  background-color: rgb(26, 26, 26);
  box-shadow: 10 10 3px rgba(99, 99, 99, 0.5);
}
</style>