<template>
  <!-- carousel -->
  <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
    <ol class="carousel-indicators">
        <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
        <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
        <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
    </ol>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="../assets/Mars.jpg" class="d-block w-100" style="width:100%" alt="Marte">
            
        <div class="carousel-caption d-none d-md-block">
          <h5>Viaje a Marte</h5>
          <p>Quieres vivir una experiencia de otro planeta... pues tenemos el plan perfecto para ti, te invitamos a conocer los detalles de 
          nuestra experiencia, dejanos tus datos y un asesor se pondrá en contacto para brindarte todos los detalles!</p>
        </div>
      </div>
      <div class="carousel-item">
        <img src="../assets/Tour.jpg" class="d-block w-100" style="width:100%" alt="Tour">
        <div class="carousel-caption d-none d-md-block">
          <h5>Tour Instalaciones</h5>
          <p>Te daremos un tour guiado pro nuestras instalaciones para que conozcas el mundo interno donde los sueños de ir a otro planeta se
          hacen realidad!</p>
        </div>
      </div>
      <div class="carousel-item">
        <img src="../assets/Shop.jpg" class="d-block w-100" style="width:100%" alt="Acccesorios">
        <div class="carousel-caption d-none d-md-block">
          <h5>Accesorios</h5>
          <p>Quieres estar equipado con todo lo que necesitas para emprender tu viaje, entra y hazte con todo lo que necesitas para estar en sintonía con la aventura.</p>
        </div>
      </div>
    </div>
    <a class="carousel-control-prev" onclick="plusSlides(-1)" href="#carouselExampleCaptions" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" onclick="plusSlides(1)" href="#carouselExampleCaptions" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
    </a>
  </div>
</template>
<script>
export default {
    name: 'CarouselSection'
 }
</script>