<template>
  <div id="app">
    <img alt="Vue super" src="./assets/yo.jpg">
    <HelloWorld msg="Bienvenido a mi portafolio"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #000000; /* Color de texto negro */
  margin-top: 60px;
  background-image: url('@/assets/fondo5.jpg');
  background-size: cover; /* Ajusta el tamaño de la imagen para cubrir todo el contenedor */
  background-position: center; /* Centra la imagen de fondo */
  background-attachment: fixed; /* Fija la imagen de fondo para que no se mueva */
}
</style>
