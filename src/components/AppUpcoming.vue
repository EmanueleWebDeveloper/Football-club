<template>
     <div>
    <AppUpcomingDinamico :matches="upcomingMatches" />
  </div>

</template>
  
  <script>
  import AppUpcomingDinamico from './AppUpcomingDinamico.vue';
  import { store } from '../store'

  
  export default {
    components: {
        AppUpcomingDinamico
    },
    name: 'AppUpcoming',
    data() {
    return {
    store,
    upcomingMatches: [
      {
        homeTeam: 'Schalke',
        awayTeam: 'Inter Club',
        homeTeamLogo: 'src/assets/league-club-1.png',
        awayTeamLogo: 'src/assets/league-club-2.png',
        matchDate: 'May 18, 2022 18:05 pm',
        stadium: 'Expert Stadium'
      },
      {
          homeTeam: 'Schalke',
          awayTeam: 'Madrid Club',
          homeTeamLogo: 'src/assets/club-3.png',
          awayTeamLogo: 'src/assets/club-4.png',
          matchDate: 'Octubre 21, 2022 19:05 pm',
          stadium: 'Expert Stadium'
        },
        {
          homeTeam: 'United Fs Club',
          awayTeam: 'Instanbul Club',
          homeTeamLogo: 'src/assets/club-6.png',
          awayTeamLogo: 'src/assets/club-7.png',
          matchDate: 'August 01, 2022 16:05 pm',
          stadium: 'Expert Stadium'
        },
        {
          homeTeam: 'Arsenal Fs Club',
          awayTeam: 'Bayer Fs Club	',
          homeTeamLogo: 'src/assets/club-8.png',
          awayTeamLogo: 'src/assets/club-9.png',
          matchDate: 'september 21, 2022 12:05 pm',
          stadium: 'Expert Stadium'
        },
        {
          homeTeam: 'Palermo',
          awayTeam: 'Catania Club',
          homeTeamLogo: 'src/assets/club-11.png',
          awayTeamLogo: 'src/assets/club-2.png',
          matchDate: 'octubre 25, 2022 20:05 pm',
          stadium: 'Expert Stadium'
        },
    
        ]
  };
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
        background-color: rgba(30, 61, 106, 0.4);
        width: 80%;
        margin: 0 auto;
    }
    .coloredue{
        background-color: rgba(21, 41, 72, 0.7);
        width: 80%;
        margin: 0 auto;
    }
}
  </style>
  
