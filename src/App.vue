<template>
  <div id="app">
    <BigChungus msg="Hello "/>
  </div>
</template>

<script>
import BigChungus from './components/BigChungus.vue'

export default {
  name: 'App',
  components: {
    BigChungus
  }
}
</script>

<style>
html, body {
  margin: 0;
  overflow: hidden;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100vw;
  height: 100vh;
  max-width: 100vw;
  max-height: 100vh;
}
</style>

