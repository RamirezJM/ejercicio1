<script setup>
</script>
<template>
  <nav>
    <h1>World Travel</h1>
    <ul>
      <li><a href="#">Nosotros</a></li>
      <li><a href="#">Lugares</a></li>
    </ul>
  </nav>
</template>

<style>
nav {
  width: 100%;
  display: flex;
  align-items: center;
  padding: 1em 2em;
  background: linear-gradient(rgb(138, 226, 138), rgb(120, 126, 120));
}

ul{
  display: flex;
  list-style-type: none;
  gap: 2em;
}

h1 {
  margin-right: auto;
}

a {
  text-decoration: none;
  color: #323232;
  font-size: 1.2rem;
}
</style>