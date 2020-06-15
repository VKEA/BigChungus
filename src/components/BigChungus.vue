<template>
  <div class="hello">
    <h1 ref="chungusMessage">{{ msg }}{{ name }}</h1>
    <input ref="chungusName" v-model="name">
    <button v-on:click="random()">Random</button>
  </div>
</template>

<script>

export default {
  name: 'BigChungus',
  props: {
    msg: String
  },
  methods: {
    random: function () {
      const names = this.names
      const name = names[Math.floor(Math.random() * names.length)]

      this.$refs.chungusName.value = name
      this.name = name
    }
  },
  data () {
    const names = [
      'Big Chugnus',
      'Grote Stukkus',
      'Big Chonker',
      'Big Chungus',
      'Big Chuggus',
      'Wing Chungus Kung Fu',
      'Extra Large Chungus',
      'Chungous Humongous'
    ]
    const name = names[Math.floor(Math.random() * names.length)]
    return {
      names: names,
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
