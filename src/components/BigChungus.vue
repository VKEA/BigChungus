<template>
  <div class="hello">
    <div class="keep-chungus-contained">
      <img ref="chungusImage" alt="Vue logo" src="../assets/Big_Chungus.png" :style="'width:'+width+';'">
    </div>
    <div class="chugnusnameholder">
      <h1 ref="chungusMessage">{{ msg }}{{ name }}</h1>
    </div>
    <input @input="resize()" ref="chungusName" v-model="name">
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
      this.$refs.chungusImage.style.width = this.name.length * 20 + 'px'
      this.name = name
    },
    resize: function () {
      this.$refs.chungusImage.style.width = this.$refs.chungusName.value.length* 20 + 'px'
    }
  },
  data () {
    const names = [
      'Big Chugnus',
      'Grote Stukkus',
      'Big Chonker',
      'Big Chungus',
      'Big Chuggus',
      'Wing Chungus',
      'Extra Large Chungus',
      'Chungous Humongous',
      'Yoshikage Chungus'
    ]
    const name = names[Math.floor(Math.random() * names.length)]
    const width = name.length * 20 + 'px'
    return {
      names: names,
      name: name,
      width: width
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
.keep-chungus-contained {
  max-width: 100%;
  height: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
}
.chugnusnameholder {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
</style>
