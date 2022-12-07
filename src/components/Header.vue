<template>
  <header>
    <img v-if="img" class="logo" alt="Csaba logo" :src="getImgUrl(img)">
    <h1>{{heading}}</h1>
  </header>
</template>

<script>
export default {
  name: 'Header',

  props: {
    heading: {
      type: String,
      default: ''
    },
    img: {
      type: String,
      required: false
    }
  },
  methods: {
    getImgUrl(image) {
      return require('../assets/'+image)
    }
  },
}
</script>

<style scoped>
header{
  padding: 4em;
}
.logo{
  width: 20%;
  border-radius: 100%;
  margin: 5em;
}
</style>
