<script setup>

</script>

<template>
  <footer>
    <div class="footer">
      <div class="texto">
        <h1>Formas de contacto</h1>
        <p>Correo: motesreyaquilino@gmail.com</p>
        <p>Teléfono: 600 815 960</p>
        <p>Instagram: Quilinoreyes_moda_</p>
        <h3>Se hacen envíos a toda España.</h3>
      </div>
    </div>
  </footer>
</template>

<style scoped>
.footer {

  padding: 40px;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 5px;
  color: goldenrod;
  font-size: 1.2rem;
  margin: 20px;
  padding-bottom: 200px;

  
}

.texto {
  width: 400%;
  border: 1px solid goldenrod;
  padding: 20px;
  border-radius: 15%;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  opacity: 0.9;
  background-color: black;
  gap: 10px;
}

@media (max-width: 900px) {

.texto{
  width: 400%;
  text-align: center;
}
}

@media (max-width: 1580px) {

.texto {
  width: 400%;
  background-color: rgb(0, 0, 0);
  opacity: 0.9;
  font-size: 1.2rem;
}
}
</style>