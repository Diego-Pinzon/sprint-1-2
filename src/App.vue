<template>
  <div id="app">
    <image-text> </image-text>
    <carousel-section> </carousel-section>
    
    <!-- news -->
    <div id="Noticias" class="container-fluid">
      <h1 class="text-center" style="italic" >Noticias</h1>
      <br>
      <news-section> </news-section>   
      </div>
    
    <!-- team -->
    <div id="Equipo" class="container-fluid">
      <h1 class="text-center" style="italic" >Nuestro Equipo</h1>
        <br>
      <div class="row justify-content-center mb-5">
        <div class="col mt-5" v-for="(integrante, id) of Equipo" :key="id">
        <team-card :member="integrante"> </team-card>
        </div>
      </div>
    </div>

    <footer-section> </footer-section>

  </div>
</template>
 
<script>

import ImageText from './components/ImageText.vue'
import CarouselSection from './components/CarouselSection.vue'
import FooterSection from './components/FooterSection.vue'
import TeamCard from './components/TeamCard.vue'
import NewsSection from './components/NewsSection.vue'
import datosequipo from '../public/datosequipo.json'

export default {
  name: 'App',
  components: {
    ImageText,
    CarouselSection,
    FooterSection,
    TeamCard,
    NewsSection
  },
  computed: {
    Equipo() {
      return datosequipo.Equipo.map((miembros) => {
        return miembros;
      })
    }
  }
}
</script>,
    

