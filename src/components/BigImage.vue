<template>
  <img alt="He is Big Chungus" :src="img">
</template>

<script>
export default {
  name: 'BigImage',
  props: {
    img: String
  }
}
</script>

<style scoped>
img {
  width: 200px;
}
</style>
