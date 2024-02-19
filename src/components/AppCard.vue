<template>
    <h2 class="d-flex justify-content-center">PLAYERS</h2>
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
    <div class="d-flex justify-content-center p-3">
        <button type="button" class=" btn btn-dark btn-lg btn-border-radius">View All Player</button>
    </div>

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
  </style>
  
