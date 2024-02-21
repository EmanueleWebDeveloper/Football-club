<template>
<div id="carouselExampleCaptions" class="carousel slide">

  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="../assets/slider1-1.jpg" class="d-block w-100" style="height: 700px;"  alt="...">
      <div class="carousel-caption d-none d-md-block py-5">
        <h2 style="font-size: 70px;">Football Club <br> Sport Club</h2>        
        <p class="fs-3">Private football matches</p>
        <button type="button" class="btn btn-lg btn-outline-light">Learn More</button>
      </div>
    </div>
    <div class="carousel-item">
      <img src="../assets/slider2-1.jpg" class="d-block w-100" style="height: 700px;" alt="...">
      <div class="carousel-caption d-none d-md-block py-5">
        <h5 style="font-size: 70px;">La tua squadra Preferita</h5>
        <p class="fs-3">Dove vuoi!</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="../assets/slider3.jpg" class="d-block w-100" style="height: 700px;" alt="...">
      <div class="carousel-caption d-none d-md-block py-5">
        <h5 style="font-size: 70px;">Isciviti Subito!</h5>
        <p class="fs-3">Non perdere l'occasione di vincere meravigliosi premi.</p>
      </div>
    </div>
    <div class="carousel-item">
      <img src="../assets/slider4.jpg" class="d-block w-100" style="height: 700px;" alt="...">
      <div class="carousel-caption d-none d-md-block py-5">
        <h5 style="font-size: 70px;">Tickets</h5>
        <p class="fs-3">Acquista qui il tuo biglietto</p>
        <button type="button" class="btn btn-lg btn-outline-light">Compra Tickets</button>
      </div>
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
</template>
  
  <script>
  
  export default {
    name: 'AppCarosello',
    data() {
        return {
  
    };
  },
  
};
</script>
  
  <style lang="scss" scoped>

  </style>
  
