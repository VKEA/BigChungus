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
    msg: String
  },
  data () {
    const names = [
      'Big Chugnus',
      'Grote Stukkus',
      'Big Chonker',
      'Big Chungus',
      'Big Chuggus'
    ]
    const name = names[Math.floor(Math.random() * names.length)]
    return {
      name: name
    }
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
