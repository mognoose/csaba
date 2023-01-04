<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/links">Links</router-link> |
    <a target="_blank" href="http://sapatti.synology.me:5000/">NAS</a> |
    <a target="_blank" href="http://sapatti.synology.me:8123">Home Assistant</a>
    |
    <a target="_blank" href="http://sapatti.synology.me:8080/photo">Photos</a>
  </nav>
</template>

<script>
export default {
  name: "Navi",
};
</script>
