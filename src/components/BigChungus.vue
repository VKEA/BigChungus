<template>
  <div class="hello">
    <h1>{{ msg }}{{ name }}</h1>
    <input v-model="name">
  </div>
</template>

<script>
export default {
  name: 'BigChungus',
  props: {
    msg: String,
    name: String
  }
}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
