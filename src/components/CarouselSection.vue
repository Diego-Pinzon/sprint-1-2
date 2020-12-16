<template>
  <div id="Servicios">
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="3000"
      controls
      indicators
      background="#ccc"
      img-width="1024"
      img-height="480"
      style="text-shadow: 1px 1px 2px #000;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image -->
      <b-carousel-slide
        caption="Viaje a Marte"
        text="Quieres vivir una experiencia de otro planeta... pues tenemos el plan perfecto para ti, te invitamos a conocer los detalles de 
        nuestra experiencia, agenda tu cita y un asesor se pondrá en contacto para brindarte todos los detalles!"
        img-src="https://imgur.com/sONFIr2.jpg"
      ></b-carousel-slide>

      <b-carousel-slide
        caption="Tour Instalaciones"
        text="Te daremos un tour guiado pro nuestras instalaciones para que conozcas el mundo interno donde los sueños de ir a otro planeta se
        hacen realidad!"
        img-src="https://i.imgur.com/uGYEijk.jpg"
      ></b-carousel-slide>
      <b-carousel-slide
        caption="Accesorios"
        text="Quieres estar equipado con todo lo que necesitas para emprender tu viaje, entra y hazte con todo lo que necesitas para estar en sintonía con la aventura."
        img-src="https://i.imgur.com/cGBvWri.jpg"
      ></b-carousel-slide>

    </b-carousel>
  </div>
</template>

<script>
    export default {
        name: 'CarouselSection',
        data() {
            return {
                slide: 0,
                sliding: null
            }
        },
        methods: {
            onSlideStart() {
                this.sliding = true
            },
            onSlideEnd() {
                this.sliding = false
            }
        }
    }
</script>