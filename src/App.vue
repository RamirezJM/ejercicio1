<script setup>
import { ref } from 'vue'
import datos from '../src/assets/data.json'
import Tarjeta from './components/Tarjeta.vue';
import Nav from './components/Nav.vue';

const lugares = ref(datos)

</script>

<template>
  <Nav />
  <main>

    <h2>Nuestros destinos</h2>
    <Tarjeta v-for="({ id, name, country, continent, image }) in lugares" :key="id" :name="name" :country="country"
      :continent="continent" :image="image" />

  </main>
</template>

<style>
h2 {
  margin: 2em auto;
  grid-column: 1/-1;
}

main {
  width: 90%;
  margin: 0 auto;
  padding: 1em;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 1em;
}
</style>
