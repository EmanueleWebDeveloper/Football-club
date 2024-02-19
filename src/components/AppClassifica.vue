<template>
  <div class="d-flex justify-content-around pt-3">
    <h2>League Table</h2>
    <h2>Fixtures and Results</h2>
  </div>
  <div class="d-flex justify-content-center">

    <div class="col-6 ">
      <div  class=" table-responsive table-responsive-lg p-4 ms-3">
        <table class="table table-lg ">
          <thead>
            <tr class="sfondo">
              <th>TEAM</th>
              <th>W</th>
              <th>D</th>
              <th>L</th>
              <th>PTS</th>
            </tr>
          </thead>
          <tbody style="height: 536px;">
            <tr v-for="team in teams" :key="team.name">
              <td>{{ team.name }}</td>
              <td>{{ team.vittorie }}</td>
              <td>{{ team.pareggi }}</td>
              <td>{{ team.sconfitte }}</td>
              <td>{{ calcolaPunti(team) }}</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>

    <div class="col-6 mt-4 mb-5 me-5  ">
      <div class="d-flex justify-content-center  align-items-center sfondodx">
        <div class="d-flex align-items-center">
          <h5>United Fs Club</h5>
          <img class="imgx" src="../assets/club-1.png"  alt="">
        </div>
        <h2 class="bold px-3">VS</h2>
        <div class="d-flex align-items-center">
          <img class="imgx" src="../assets/club-2.png" alt="">
          <h5>Instanbul Sports</h5>
        </div>
      </div>

      <div class="d-flex justify-content-center p-1 align-items-center sfondodxdue">
        <div class="d-flex align-items-center">
          <h5>Schalke Club</h5>
          <img class="imgx" src="../assets/club-3.png"  alt="">
        </div>
        <h2 class="bold px-3">VS</h2>
        <div class="d-flex align-items-center">
          <img class="imgx" src="../assets/club-4.png" alt="">
          <h5>Inter Club</h5>
        </div>
      </div>

      <div class="d-flex justify-content-center p-1 align-items-center sfondodx">
        <div class="d-flex align-items-center">
          <h5>Madrid Club</h5>
          <img class="imgx" src="../assets/club-8.png"  alt="">
        </div>
        <h2 class="bold px-3">VS</h2>
        <div class="d-flex align-items-center">
          <img class="imgx" src="../assets/club-6.png" alt="">
          <h5>United Fs Club</h5>
        </div>
      </div>

      <div class="d-flex justify-content-center p-1 align-items-center sfondodxdue">
        <div class="d-flex align-items-center">
          <h5>Arsenal Fs Club</h5>
          <img class="imgx" src="../assets/club-7.png"  alt="">
        </div>
        <h2 class="bold px-3">VS</h2>
        <div class="d-flex align-items-center">
          <img class="imgx" src="../assets/club-8.png" alt="">
          <h5>Bayer Fs Club</h5>
        </div>
      </div>

      <div class="d-flex justify-content-center p-1 align-items-center sfondodx">
        <div class="d-flex align-items-center">
          <h5>Atletico Fs Club</h5>
          <img class="imgx" src="../assets/club-9.png"  alt="">
        </div>
        <h2 class="bold px-3">VS</h2>
        <div class="d-flex align-items-center">
          <img class="imgx" src="../assets/club-11.png" alt="">
          <h5>Instanbul Sports</h5>
        </div>
      </div>
      <div class="d-flex justify-content-center p-1 align-items-center sfondodxdue">
        <div class="d-flex align-items-center">
          <h5>Catania</h5>
          <img class="imgx" src="../assets/club-11.png"  alt="">
        </div>
        <h2 class="bold px-3">VS</h2>
        <div class="d-flex align-items-center">
          <img class="imgx" src="../assets/club-2.png" alt="">
          <h5>Palermo Sports</h5>
        </div>
      </div>
      <div class="d-flex justify-content-center p-1 align-items-center sfondodx">
        <div class="d-flex align-items-center">
          <h5>Roma ss</h5>
          <img class="imgx" src="../assets/club-4.png"  alt="">
        </div>
        <h2 class="bold px-3">VS</h2>
        <div class="d-flex align-items-center">
          <img class="imgx" src="../assets/club-7.png" alt="">
          <h5>Miami Sports</h5>
        </div>
      </div>
      <div class="d-flex justify-content-center p-1 align-items-center sfondodxdue">
        <div class="d-flex align-items-center">
          <h5>acapulco</h5>
          <img class="imgx" src="../assets/club-3.png"  alt="">
        </div>
        <h2 class="bold px-3">VS</h2>
        <div class="d-flex align-items-center">
          <img class="imgx" src="../assets/club-11.png" alt="">
          <h5>gergi Sports</h5>
        </div>
      </div>

      <div class="d-flex justify-content-center p-1 align-items-center sfondodx">
        <div class="d-flex align-items-center">
          <h5>Dortmund</h5>
          <img class="imgx" src="../assets/club-11.png"  alt="">
        </div>
        <h2 class="bold px-3">VS</h2>
        <div class="d-flex align-items-center">
          <img class="imgx" src="../assets/club-2.png" alt="">
          <h5>Barcellona Sports</h5>
        </div>
      </div>

      
    </div>

    
  </div>

  <div>
    <img src="../assets/reklam.jpg" alt="">
  </div>
  
</template>

<script>

export default {
  name: 'AppClassifica',
  data() {
    return {
      teams: [
        { name: 'Instanbul', vittorie: 18, pareggi: 2, sconfitte: 0 },
        { name: 'United Fs Club', vittorie: 14, pareggi: 2, sconfitte: 1 },
        { name: 'Schalke Club', vittorie: 13, pareggi: 3, sconfitte: 1 },
        { name: 'Inter Club', vittorie: 13, pareggi: 2, sconfitte: 1 },
        { name: 'Madrid Club', vittorie: 12, pareggi: 2, sconfitte: 1 },
        { name: 'United Fs Club', vittorie: 11, pareggi: 2, sconfitte: 1 },
        { name: 'Arsenal Fs Club', vittorie: 10, pareggi: 2, sconfitte: 1 },
        { name: 'Bayer Fs Club', vittorie: 9, pareggi: 2, sconfitte: 1 },
        { name: 'Atletico Fs Club', vittorie: 8, pareggi: 2, sconfitte: 1 }
      ]
    }
  },
  methods: {
    calcolaPunti: function(team) {
      return team.vittorie * 3 + team.pareggi;
      
    }
  }
};
</script>

<style lang="scss" scoped>
th{
  background-color: black;
  color: white;
  padding: 10px;
}
td{
  background-color:#f5f5f5
 ;
}
.sfondodx{
  background-color:#ebebeb

}
.sfondodxdue{
  background-color: #f3f3f3;
}
.imgx{
  width: 50px;
}
.altezza{
  width: 100%;
}
</style>
