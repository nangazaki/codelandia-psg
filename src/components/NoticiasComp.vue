<template>
  <section class="noticias flex">
    <div class="container">
      <h3>Ultimas notícias</h3>
      <div class="noticias-container flex">
        <CardNoticiaComp
          v-for="(noticia, key) in noticias" :key="key"
          :img="require(`../assets/img/${noticia.imagem}`)"
          :titulo="noticia.titulo"
          :marcador="noticia.marcador"
        :data="noticia.data"/>
      </div>
      <div class="btn-section">
        <ButtonComp link="#" name="carregar mais"/>
      </div>
    </div>
  </section>
</template>

<script>
import CardNoticiaComp from './CardNoticiaComp.vue'
import ButtonComp from './ButtonComp.vue';
export default {
    name: "NoticiasComp",
    components: { CardNoticiaComp, ButtonComp },
    data() {
        return {
            noticias: [
                {
                    imagem: "image3.png",
                    titulo: "Messi deseja comprar 35% das ações de clube.",
                    marcador: "Equipa principal",
                    data: "17 Maio 2022"
                },
                {
                    imagem: "image4.png",
                    titulo: "Tudo sobre a vitória em Montpellier.",
                    marcador: "Equipa principal",
                    data: "15 Maio 2022"
                },
                {
                    imagem: "image5.png",
                    titulo: "Mbappe no Liverpool?",
                    marcador: "Equipa principal",
                    data: "15 Maio 2022"
                }
            ]
        };
    }
}
</script>