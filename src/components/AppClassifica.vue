<template>
  <div class="d-flex justify-content-center">
    <div class="col-6 ">
      <div class=" table-responsive table-responsive-lg ">
        <table class="table table-lg">
          <thead>
            <tr class="text-light bg-dark">
              <th>TEAM</th>
              <th>W</th>
              <th>D</th>
              <th>L</th>
              <th>PTS</th>
            </tr>
          </thead>
          <tbody>
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

    <div class="col-6">
      <div v-for="team in teams" :key="team.name" class="d-flex justify-content-center">
        <div>
          <h3>{{ team.name }}</h3>
          <img src="../../assets/club-1.png" alt="">
        </div>
        <h2 class="bold">VS</h2>
        <div>
          <img src="../../assets/club-2.png" alt="">
          <h3>Instanbul Sports </h3>
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


</style>
