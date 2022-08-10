<template>
  <div>
    <HeaderComp/>
  </div>
</template>

<script>
import HeaderComp from '@/components/HeaderComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
  }
}
</script>

<style lang="scss">
  @import './assets/scss/style.scss'
</style>