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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

