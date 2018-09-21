<template lang="pug">
  div
    dm-header
    nuxt
    dm-footer
</template>

<script>
  import DmHeader from '../components/Header.vue'
  import DmFooter from '../components/Footer.vue'

  export default {
    components: { DmHeader, DmFooter }
  }

</script>

<style>
</style>

