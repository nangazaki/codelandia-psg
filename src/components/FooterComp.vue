<template>
  <footer>
    <div class="footer container flex">
      <div>
        <span class="footer-titulo">Linguas</span>
        <div class="footer-list flex">
          <a v-for="(lingua, key) in linguas" :key="key" :href="lingua.link">
            {{ lingua.nome }}
          </a>
        </div>
      </div>
      <div>
        <span class="footer-titulo">Redes Sociais</span>
        <div class="footer-list flex">
          <a v-for="(social, key) in socialmedia" :key="key" :href="social.link">
            {{ social.nome }}
          </a>
        </div>
      </div>
      <div>
        <span class="footer-titulo">Clube</span>
        <div class="footer-list">
          <a v-for="(a, key) in clube" :key="key" :href="a.link">
            {{a.nome}}
          </a>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComp',
  data() {
    return {
      linguas: [
        {nome: 'English', link: '#'},
        {nome: 'Français', link: '#'},
        {nome: 'Español', link: '#'},
        {nome: 'العربية', link: '#'},
        {nome: 'Bahasa Indonesia', link: '#'},
        {nome: '中文', link: '#'}
      ],
      socialmedia: [
        {nome: 'Facebook', link: '#'},
        {nome: 'YouTube', link: '#'},
        {nome: 'Instagram', link: '#'}
      ],
      clube: [
        {nome: 'Patrocinadores', link: '#'}
      ]
    }
  },
}
</script>