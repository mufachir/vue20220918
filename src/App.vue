<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/mufachir.jpg" style="width: 150px; height: 150px; border-radius: 50%">
    <HelloWorld msg="Welcome to my Personal Website"/>
  </div>
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
</style>
