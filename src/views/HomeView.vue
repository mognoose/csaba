<template>
  <div class="content">
    <Header heading="Csaba Szilagyi" img="logo.jpg"/>
    <NasButtons/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import NasButtons from '@/components/NasButtons.vue'

export default {
  name: 'HomeView',
  components: {
    Header,
    NasButtons,
  }
}
</script>
