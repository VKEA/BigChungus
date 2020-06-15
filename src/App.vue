<template>
  <div id="app">
    <BigImage img="https://vignette.wikia.nocookie.net/david-and-friends/images/c/c4/Big_Chungus.png/revision/latest?cb=20190516074316"/>
    <BigChungus msg="Hello "/>
  </div>
</template>

<script>
import BigChungus from './components/BigChungus.vue'
import BigImage from './components/BigImage.vue'

export default {
  name: 'App',
  components: {
    BigChungus,
    BigImage
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
