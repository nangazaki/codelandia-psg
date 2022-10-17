<template>
  <div class="header">
    <div class="container">
      <NavbarComp/> 
      <article>
        <h1>Neymar JR</h1>
        <p>
          "Tenho Messi e Ronaldo como ídolos.
          Se der para pegar um pouquinho de
          cada um, fico muito feliz."
        </p>
        <ButtonComp 
          href="#"
          name="ler matéria"
        />
      </article> 
    </div>
  </div>
</template>

<script>
import ButtonComp from './ButtonComp.vue'
import NavbarComp from './NavbarComp.vue'

export default {
  name: 'HeaderComp',
  components: {
    NavbarComp,
    ButtonComp
}
}
</script>