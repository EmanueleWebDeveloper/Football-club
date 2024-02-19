<template>
    <section class="p-5">
        <div class="d-flex gap-3 justify-content-center text-uppercase fs-2  align-items-center">
            <div class="d-flex align-items-center">
                <h3>Instanbul Sports </h3>
                <img src="../assets/club-1.png"  alt="">
            </div>
            <h2 class="fs-1">VS</h2>
            <div class="d-flex align-items-center">
                <img src="../assets/club-2.png" alt="">
                <h3>Instanbul Sports </h3>
            </div>

        </div>


        <div class="d-flex gap-3 justify-content-center ">
        <h5>May 21,2022 18:05 pm</h5>  
        <h5>Expert Stadium</h5>   
        </div>

        <div class="d-flex justify-content-center text-uppercase pt-4">
            <button type="button" class="btn btn-dark btn-lg">View Match Details</button>

        </div>

        
    </section>

</template>
  
  <script>
  
  import { store } from '../store'

  
  export default {
    name: 'AppMain',
    data() {
      return {
        store
      }
    }
  }
  </script>
  
  <style lang="scss" scoped>
 img{
  width: 100px;
 }
  </style>
  
