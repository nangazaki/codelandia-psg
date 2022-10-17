<template>
  <div class="card">
    <div class="card-img">
      <img :src="img">
    </div>
    <div class="card-info">
      <div class="card-marcador flex">
        <span>{{ marcador }}</span>
        <span>{{ data }}</span>
      </div>
      <div class="card-link">
        <a href="#"> {{ titulo }} </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardNoticiaComp',
  props: {
    img: String,
    titulo: String,
    marcador: String,
    data: String
  }
}
</script>