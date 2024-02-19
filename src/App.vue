<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";
import AppUpcoming from "./components/AppUpcoming.vue";
import AppCard from "./components/AppCard.vue";
import AppClassifica from "./components/AppClassifica.vue";
import AppSponsor from "./components/AppSponsor.vue";
import AppFooter from "./components/AppFooter.vue";
import AppCarosello from "./components/AppCarosello.vue";




import { store } from "./store";
import axios from "axios";

export default {
  components: {
    AppHeader,
    AppMain,
    AppUpcoming,
    AppCard,
    AppClassifica,
    AppSponsor,
    AppFooter,
    AppCarosello
},
  data() {
    return {
      store,
    };
  },

};
</script>

<template>
  <AppHeader/>
  <AppCarosello/>
  <AppMain/>
  <AppUpcoming/>
  <AppCard/>
  <AppClassifica/>
  <AppSponsor/>
  <AppFooter/>
</template>

<style lang="scss">
@use "./styles/general.scss";


</style>
