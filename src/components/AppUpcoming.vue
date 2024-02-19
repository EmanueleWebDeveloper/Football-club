<template>
    <section>
        
        <div class="sfondo">
            <h2 class="d-flex gap-3 justify-content-center text-white py-4">Upcoming Matchs</h2>
            <div class="lex-column gap-3 justify-content-center text-uppercase fs-2  align-items-center text-white py-4">

                <div class="d-flex gap-3 justify-content-center  px-5  colore ">

                    <div class="d-flex align-items-center ">
                        <h3>Schalke  </h3>
                        <img src="../assets/club-1.png" alt="">
                    </div>
                    <h2 class="fs-1">VS</h2>
                    <div class="d-flex align-items-center">
                        <img src="../assets/club-2.png" alt="">
                        <h3>Inter Club </h3>
                    </div>   
                </div>
                <div class="d-flex gap-3 justify-content-center text-white coloredue ">
                <h5>May 21,2022 18:05 pm</h5>  
                <h5>Expert Stadium</h5>   
                </div> 
            </div>
            <div class="lex-column gap-3 justify-content-center text-uppercase fs-2  align-items-center text-white py-4">

<div class="d-flex gap-3 justify-content-center  px-5  colore ">

    <div class="d-flex align-items-center ">
        <h3>Schalke  </h3>
        <img src="../assets/club-3.png" alt="">
    </div>
    <h2 class="fs-1">VS</h2>
    <div class="d-flex align-items-center">
        <img src="../assets/club-4.png" alt="">
        <h3>Inter Club </h3>
    </div>   
</div>
<div class="d-flex gap-3 justify-content-center text-white coloredue ">
<h5>May 21,2022 18:05 pm</h5>  
<h5>Expert Stadium</h5>   
</div> 
</div>

<div class="lex-column gap-3 justify-content-center text-uppercase fs-2  align-items-center text-white py-4">

<div class="d-flex gap-3 justify-content-center  px-5  colore ">

    <div class="d-flex align-items-center ">
        <h3>Schalke  </h3>
        <img src="../assets/club-11.png" alt="">
    </div>
    <h2 class="fs-1">VS</h2>
    <div class="d-flex align-items-center">
        <img src="../assets/club-6.png" alt="">
        <h3>Inter Club </h3>
    </div>   
</div>
<div class="d-flex gap-3 justify-content-center text-white coloredue ">
<h5>May 21,2022 18:05 pm</h5>  
<h5>Expert Stadium</h5>   
</div> 
</div>

<div class="lex-column gap-3 justify-content-center text-uppercase fs-2  align-items-center text-white py-4">

<div class="d-flex gap-3 justify-content-center  px-5  colore">

    <div class="d-flex align-items-center ">
        <h3>Schalke  </h3>
        <img src="../assets/club-7.png" alt="">
    </div>
    <h2 class="fs-1">VS</h2>
    <div class="d-flex align-items-center">
        <img src="../assets/club-8.png" alt="">
        <h3>Inter Club </h3>
    </div>   
</div>
<div class="d-flex gap-3 justify-content-center text-white coloredue ">
<h5>May 21,2022 18:05 pm</h5>  
<h5>Expert Stadium</h5>   
</div> 
</div>

<div class="lex-column gap-3 justify-content-center text-uppercase fs-2  align-items-center text-white py-4">

<div class="d-flex gap-3 justify-content-center  px-5  colore">

    <div class="d-flex align-items-center ">
        <h3>Schalke  </h3>
        <img src="../assets/club-3.png" alt="">
    </div>
    <h2 class="fs-1">VS</h2>
    <div class="d-flex align-items-center">
        <img src="../assets/club-11.png" alt="">
        <h3>Inter Club </h3>
    </div>   
</div>
<div class="d-flex gap-3 justify-content-center text-white coloredue ">
<h5>May 21,2022 18:05 pm</h5>  
<h5>Expert Stadium</h5>   
</div> 
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
  .sfondo{
    background-image: url("../assets/saha.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center; 


    .colore{
        background-color: #1e3d6a;
        width: 80%;
        margin: 0 auto;
    }
    .coloredue{
        background-color: #152948;
        width: 80%;
        margin: 0 auto;
    }
}
  </style>
  
