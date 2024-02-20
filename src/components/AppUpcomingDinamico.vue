<template>
    <section>
      <div class="sfondo pb-5">
        <h2 class="d-flex gap-3 justify-content-center text-white py-4">Upcoming Matches</h2>
        <div v-for="(match, index) in matches" :key="index">
          <div class="  justify-content-center text-uppercase fs-2 align-items-center text-white py-2">
            
            <div class="d-flex gap-5 justify-content-center px-5 align-items-center colore p-1">
              <div class="d-flex align-items-center">
                  <img :src="match.homeTeamLogo" alt="">
                <h3>{{ match.homeTeam }}</h3>
              </div>
              <h2 class="fs-1">VS</h2>
              <div class="d-flex align-items-center">
                  <h3>{{ match.awayTeam }}</h3>
                <img :src="match.awayTeamLogo" alt="">
              </div>
            </div>
            <div class="d-flex gap-3 justify-content-center text-white coloredue">
              <h5>{{ match.matchDate }}</h5>
              <h5>{{ match.stadium }}</h5>
            </div>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    props: {
      matches: Array
    }
  };
  </script>
  
  <style scoped>
.sfondo{
    background-image: url("../assets/saha.jpg");
    background-repeat: no-repeat;
    background-size: 100% 100%;
    background-position: center; 


    .colore{
        background-color: rgba(30, 61, 106, 0.4);
        width: 80%;
        margin: 0 auto;
    }
    .coloredue{
        background-color: rgba(21, 41, 72, 0.7);
        width: 80%;
        margin: 0 auto;
    }
    img{
        width: 150px;
    }
}
  </style>
  