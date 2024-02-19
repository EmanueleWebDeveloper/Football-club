<template>
    <section>
    <h2 class="d-flex gap-3 justify-content-center">Upcoming Matchs</h2>
    
        <div class="">
            <div class="d-flex gap-3 justify-content-center text-uppercase fs-2  align-items-center opacity-75">
                <div class="d-flex align-items-center">
                    <h3>Schalke  </h3>
                    <img src="../assets/club-1.png" alt="">
                </div>
                <h2 class="fs-1">VS</h2>
                <div class="d-flex align-items-center">
                    <img src="../assets/club-2.png" alt="">
                    <h3>Inter Club </h3>
                </div>   
            </div>
            <div class="d-flex gap-3 justify-content-center ">
            <h5>May 21,2022 18:05 pm</h5>  
            <h5>Expert Stadium</h5>   
            </div> 

            <div class="d-flex gap-3 justify-content-center text-uppercase fs-2  align-items-center opacity-75">
                <div class="d-flex align-items-center">
                    <h3>Atletico Club  </h3>
                    <img src="../assets/club-3.png" alt="">
                </div>
                <h2 class="fs-1">VS</h2>
                <div class="d-flex align-items-center">
                    <img src="../assets/club-4.png" alt="">
                    <h3>Schalke  </h3>
                </div>   
            </div>
            <div class="d-flex gap-3 justify-content-center ">
            <h5>May 21,2022 18:05 pm</h5>  
            <h5>Expert Stadium</h5>   
            </div> 

            <div class="d-flex gap-3 justify-content-center text-uppercase fs-2  align-items-center opacity-75">
                <div class="d-flex align-items-center">
                    <h3>United Sports </h3>
                    <img src="../assets/club-2.png" alt="">
                </div>
                <h2 class="fs-1">VS</h2>
                <div class="d-flex align-items-center">
                    <img src="../assets/club-6.png" alt="">
                    <h3>Bayern Sports </h3>
                </div>   
            </div>
            <div class="d-flex gap-3 justify-content-center ">
            <h5>May 21,2022 18:05 pm</h5>  
            <h5>Expert Stadium</h5>   
            </div> 

            <div class="d-flex gap-3 justify-content-center text-uppercase fs-2  align-items-center opacity-75">
                <div class="d-flex align-items-center">
                    <h3>Arsenal Club </h3>
                    <img src="../assets/club-7.png" alt="">
                </div>
                <h2 class="fs-1">VS</h2>
                <div class="d-flex align-items-center">
                    <img src="../assets/club-8.png" alt="">
                    <h3>Atletico Club </h3>
                </div>   
            </div>
            <div class="d-flex gap-3 justify-content-center ">
            <h5>May 21,2022 18:05 pm</h5>  
            <h5>Expert Stadium</h5>   
            </div> 

            <div class="d-flex gap-3 justify-content-center text-uppercase fs-2  align-items-center opacity-75">
                <div class="d-flex align-items-center">
                    <h3>Instanbul Sports </h3>
                    <img src="../assets/club-9.png" alt="">
                </div>
                <h2 class="fs-1">VS</h2>
                <div class="d-flex align-items-center">
                    <img src="../assets/club-11.png" alt="">
                    <h3>United Sports </h3>
                </div>   
            </div>
            <div class="d-flex gap-3 justify-content-center ">
            <h5>May 21,2022 18:05 pm</h5>  
            <h5>Expert Stadium</h5>   
            </div> 
        </div>


        
    </section>

</template>
  
  <script>
  
  import { store } from '../store'

  
  export default {
    name: 'AppUpcoming',
    data() {
      return {
        store
      }
    }
  }
  </script>
  
  <style lang="scss" scoped>
  section{
    background-image: url("~@/assets/reklam.jpg");  }
 
  </style>
  
