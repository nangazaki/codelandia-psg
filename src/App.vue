<template>
  <slot>
    <HeaderComp/>
    <PlacarComp/>
    <MensagemComp/>
    <NoticiasComp/>
    <FooterComp/>
  </slot>
</template>

<script>
import HeaderComp from '@/components/HeaderComp.vue'
import PlacarComp from '@/components/PlacarComp.vue'
import MensagemComp from './components/MensagemComp.vue'
import NoticiasComp from './components/NoticiasComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    PlacarComp,
    MensagemComp,
    NoticiasComp,
    FooterComp
}
}
</script>

<style lang="scss">
  @import './assets/scss/style.scss'
</style>