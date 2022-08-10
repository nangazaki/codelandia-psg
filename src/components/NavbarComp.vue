<template>
  <header>
    <a href="/">
      <img src="../assets/img/psg.svg">
    </a>
    <nav>
      <ul>
        <li v-for="(item, chave) in navlist" :key="chave">
          <a :href="item.link">
            {{ item.name }}
          </a>
        </li>
      </ul>
      <div class="btn-group">
        <a href="#">ENTRAR</a>
        <ButtonComp href="#" name="REGISTRE-SE"/>
      </div>
    </nav>
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
        {link: '/', name: 'Inicio', active: true},
        {link: '#', name: 'Resultados', active: false},
        {link: '#', name: 'Notícias', active: false},
        {link: '#', name: 'Clubes', active: false},
        {link: '#', name: 'Lojas', active: false},
      ]
    }
  }
}
</script>