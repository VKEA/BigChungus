<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/Big_Chungus.png">
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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

img {
  width: 200px;
}
</style>

