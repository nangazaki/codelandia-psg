<template>
  <header class="flex">
    <a href="/">
      <img src="../assets/img/psg.svg">
    </a>
    <nav class="flex">
      <ul class="flex">
        <li v-for="(item, chave) in navlist" :key="chave">
          <a :href="item.link">
            {{ item.name }}
          </a>
        </li>
      </ul>
      <div class="btn-group flex">
        <a href="#">ENTRAR</a>
        <ButtonComp href="#" name="REGISTRE-SE"/>
      </div>
    </nav>
    <div class="mobile-menu">
      <span>Menu</span>
      <span class="lines flex">
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
        <span class="line"></span>
      </span>
    </div>
  </header>
</template>

<script>
import ButtonComp from './ButtonComp.vue'

export default {
  name: 'NavbarComp',
  components: {
    ButtonComp
  },
  data(){
    return{
      navlist: [
        {link: '/', name: 'Inicio'},
        {link: '#', name: 'Resultados'},
        {link: '#', name: 'Notícias'},
        {link: '#', name: 'Clubes'},
        {link: '#', name: 'Lojas'}
      ]
    }
  }
}
</script>