<template>
  <div id="app">
    <image-text> </image-text>
    <carousel-section> </carousel-section>
    <services-section> </services-section>

    <!-- news -->
    <div class="container-fluid">
        <div class="row mt-md-5 mt-sm-5 mt-xs-5">
         <news-section> </news-section>   
        </div>
    </div>
    <!-- team -->
    <div class="container-fluid">
      <div class="row justify-content-center mb-5">
        <div class="col mt-5">
        <team-card> </team-card>
        </div>
      </div>
    </div>

    <footer-section> </footer-section>

  </div>
</template>
 
<script>

import ImageText from './components/ImageText.vue'
import CarouselSection from './components/CarouselSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import FooterSection from './components/FooterSection.vue'
import TeamCard from './components/TeamCard.vue'
import NewsSection from './components/NewsSection.vue'

export default {
  name: 'App',
  components: {
    ImageText,
    CarouselSection,
    ServicesSection,
    FooterSection,
    TeamCard,
    NewsSection
  }
}
</script>,
    NewsSection

