<template>
   <section class="sfondo">
    <h2 class="d-flex justify-content-center py-5">PLAYERS</h2>
    <div class="d-flex justify-content-center gap-4 ">
        <div class="card text-light bg-black" style="width: 18rem;">
           <img src="../assets/player1.jpg" class="card-img-top" alt="...">
           <div class="card-body text-center">
            <h3>07</h3>
            <h4>Adam Brown -</h4>
            <h4>Forwarder</h4>
           </div>
        </div>
        <div class="card text-light bg-black" style="width: 18rem;">
           <img src="../assets/player2.jpg" class="card-img-top" alt="...">
           <div class="card-body text-center">
            <h3>09</h3>
            <h4>Michael Kayn -</h4>
            <h4>Forwarder</h4>
           </div>
        </div>
        <div class="card text-light bg-black" style="width: 18rem;">
           <img src="../assets/player3.jpg" class="card-img-top" alt="...">
           <div class="card-body text-center">
            <h3>11</h3>
            <h4>Michael Lee - Forwarder</h4>
           </div>
        </div>
        <div class="card text-light bg-black" style="width: 18rem;">
           <img src="../assets/player4.jpg" class="card-img-top" alt="...">
           <div class="card-body text-center">
            <h3>15</h3>
            <h4>Ethan Smith - Midfielder</h4>
           </div>
        </div>
    </div>
    <div class="d-flex justify-content-center p-3 py-5">
        <button type="button" class=" btn btn-dark btn-lg btn-border-radius">View All Player</button>
    </div>
   </section>
</template>
  
  <script>
  
  import { store } from '../store'

  
  export default {
    name: 'AppCard',
    data() {
      return {
        store
      }
    }
  }
  </script>
  
  <style lang="scss" scoped>
  .btn{
   border-radius: 20px;
   border: 2px solid white;
  }
  .sfondo{
   background-image: url("https://www.truenumbers.it/wp-content/uploads/2021/12/football-soccer-ball-on-grass-field-2021-09-01-21-45-14-utc.jpg");
   background-repeat: no-repeat;
    background-size: cover;
    filter: brightness(0.8) contrast(1.2); 

  }
  </style>
  
