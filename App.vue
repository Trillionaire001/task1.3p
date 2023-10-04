<template>
  <HelloWorld msg="Rishabh setia"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

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
  color: #2c3e50;
  margin-top: 60px;
}

body {
  background-color: #C0C0C0; 
}

.image-container {
  display: inline-block;
  padding: 20px; 
  background-image: linear-gradient(45deg, #FF5733, #00008B); 
}
</style>
