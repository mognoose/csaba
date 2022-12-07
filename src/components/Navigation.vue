<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/links">Links</router-link> |
    <a target="_blank" href="http://sapatti.synology.me:5000/">NAS</a> |
    <a target="_blank" href="http://sapatti.synology.me:8080/photo">Photos</a>
  </nav>
</template>

<script>
export default {
  name: 'Navi',
}
</script>

<style lang="scss">
nav {
  padding: .5em;
  background-color: rgba(0,0,0,0.9);
  backdrop-filter: blur(50px);
  box-shadow: 0px 5px 10px rgba(0,0,0,0.9);


  a {
    font-weight: 400;
    color: #a9a9a9;

    &.router-link-exact-active {
      color: #54ddf5;
    }
  }
}
</style>
