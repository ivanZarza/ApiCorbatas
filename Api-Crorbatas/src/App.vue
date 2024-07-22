<script setup>
import { ref } from 'vue'
import { items } from '@/corbatas/data'
</script>

<template>

<pre><code>{{ items }}</code></pre>

</template>

<style scoped>

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-image: url('../public/photo_2024-07-22_20-44-11.jpg');
  background-size: cover;
  background-repeat:repeat;
  background-attachment: fixed;
  background-position: center;
  background-color: #000;
}

</style>
