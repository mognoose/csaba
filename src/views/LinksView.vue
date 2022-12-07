<template>
  <div class="content">
    <Header heading="Links"/>
    <div class="block">
      <p>
        <a target="_blank" href="https://www.linkedin.com/in/csaba-szilagyi/">linkedin.com</a> - My linkedin profile
      </p>
      <p>
        <a target="_blank" href="https://github.com/mognoose">github.com</a> - My github repository
      </p>
    </div>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'

export default {
  name: 'HomeView',
  components: {
    Header,
  }
}
</script>