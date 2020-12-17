<template>
  <div id="app">
    <image-text> </image-text>
    <carousel-section> </carousel-section>
    
    <!-- news -->
    <div id="news" class="container-fluid">
      <h1 class="text-center news" style="italic" >Noticias</h1>
      <br>
      <news-section> </news-section>   
      </div>
    
    <!-- team -->
    <div id="team" class="container-fluid">
      <h1 class="text-center news" style="italic" >Nuestro Equipo</h1>
        <br>
      <div class="row justify-content-center mb-5">
        <div class="col mt-5" v-for="(integrante, id) of team" :key="id">
        <team-card v-bind:member="integrante"> </team-card>
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

export default {
  name: 'App',
  components: {
    ImageText,
    CarouselSection,
    FooterSection,
    TeamCard,
    NewsSection
  },
  data(){
    return{
      team:[
      {
        codigo: 1,
        nombre: "Nilson Nicolas Vijalba Caballero",
        descripcion: "Ingeniero en automatización, experencia en desarrollo de pyhton, php, conocimientos en robotica y control industrial.",
        rol: "Programador",
        image: "https://i.imgur.com/j4lJwq6.jpg",
        whatsapp: "https://api.whatsapp.com/send?phone=573208433176",
        facebook: "https://m.me/nicovijalba"
      },
      {
        codigo: 2,
        nombre: "Diego Alexander Pinzón Mendivelso",
        descripcion: "Ingeniero Aeronáutico, con experiencia en Quality Control, Quality Assurance y Compliance en la industria aérea colombiana.",
        rol: "Programador",
        image: "https://i.imgur.com/FCmEGJ0.png",
        whatsapp: "https://api.whatsapp.com/send?phone=573007040873",
        facebook: "https://m.me/nicovijalba"
      },
      {
        codigo: 3,
        nombre: "Juan Sebastián González Rojas",
        descripcion: "Ingeniero Electrónico.  Apasionado por la ciencia, la Ingeniería, el dibujo y aprender cosas nuevas.",
        rol: "Programador",
        image: "https://i.imgur.com/rwTZ74g.jpg",
        whatsapp: "https://api.whatsapp.com/send?phone=573176550376",
        facebook: "https://m.me/nicovijalba"
      }
    ]
    }
  }
}
</script>,
<style>
.news {
  margin-top : 5%;
}
</style>
    

