<template>
  <a :href="link">
    {{ name }}
  </a>
</template>

<script>
export default {
  name: 'ButtonComp',
  props: {
    link: String,
    name: String
  }
}
</script>

<style lang="scss" scoped>
a {
  padding: 12px;
  border-radius: 4px;
  background: #DA2535;
  font-weight: 500;
  text-transform: uppercase;
}
</style>