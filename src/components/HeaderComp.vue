<template>
  <div class="header">
    <NavbarComp/> 
    <article>
      <h1>Neymar JR</h1>
      <p>
        "Tenho Messi e Ronaldo como ídolos.<br>
        Se der para pegar um pouquinho de<br> 
        cada um, fico muito feliz."
      </p>
      <ButtonComp 
        href="#"
        name="ler matéria"
      />
    </article> 
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