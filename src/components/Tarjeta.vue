<script setup>

defineProps({
  name: String,
  country: String,
  continent: String,
  image: String
})

</script>

<template>
  <article>
    <h3>{{ name }}</h3>
    <p>País: {{ country }}</p>
    <p>Continente:  {{ continent }}</p>
    <img :src="image" :alt="name">
  </article>

</template>

<style>
article{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  gap: 1em;
  border: solid 2px #424242;
  border-radius: 5px;
  padding: 1em;
  background-color: antiquewhite;

}

h3{
  text-align: center;
}

img{
  display: block;
  width: 100%;
  aspect-ratio: 1.5/1;
  object-fit: cover;
}

</style>
