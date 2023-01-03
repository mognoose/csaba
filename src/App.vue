<template class="main">
  <Navigation/>
  <router-view/>
</template>

<script>
import Navigation from '@/components/Navigation.vue'

export default {
  name: 'AppView',
  components: {
    Navigation
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700;900&display=swap');

html, body {
    margin: 0;
    padding: 0;
}
#app {
  background: url('@/assets/code.jpg') 100% 100% fixed;
  font-family: 'Roboto', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #cacaca;
  text-align: center;
  padding: 0px;
  margin: 0px;
  min-height: 100vh;
}

h1{
  color: #fff;
  text-shadow: 0px 0px 6px rgba(0,0,0,0.9);
}

a:link,
a:active,
a:visited,
a:hover {
  color: #fff;
}

.block {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    background-color: rgba(0,0,0,0.3);
    backdrop-filter: blur(50px);
    padding-top: 10em; 
    padding-bottom: 10em;
    @media (min-width: 421px){
      *:nth-child(1){
        grid-column-start: 2;
      }
      *:nth-child(2){
        grid-column-start: 3;
      }
    }
    @media (max-width: 420px) {
      grid-template-columns: 1fr;
    }
}

.content {
  margin: 0;
  padding: 0;
}
</style>
