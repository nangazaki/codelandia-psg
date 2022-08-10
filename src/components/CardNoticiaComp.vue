<template>
  <div>
    <div>
      <img :src="img">
    </div>
    <div>
      <div>
        <span>EQUIPE PRINCIPAL</span>
        <span>DATA</span>
      </div>
      <h3> {{titulo}} </h3>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardNoticiaComp',
  props: {
    img: Image,
    titulo: String
  }
}
</script>