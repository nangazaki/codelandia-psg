<template>
  <a :href="link">
    <button>{{ name }}</button>
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

  button {
    color: #f9f9f9;
    padding: 12px;
    border: none;
    border-radius: 4px;
    background: #DA2535;
    font-weight: 500;
    text-transform: uppercase;
    cursor: pointer;

    &:hover {
      background: #c21e2c;
      transition: cubic-bezier(0.075, 0.82, 0.165, 1);
    }

    @media screen and (max-width: 425px) {
      width: 100%;
    }
  }


}
</style>