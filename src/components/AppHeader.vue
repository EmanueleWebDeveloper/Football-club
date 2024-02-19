<template>
  <header class="p-3 text-light ">
    <div class="d-flex justify-content-center">
            <ul class="d-flex justify-content-center gap-3 align-items-center">
             <li>
                <img src="../assets/sponsor1.png" alt="">
                </li>
             <li>
                 <img src="../assets/sponsor2.png" alt="">
                </li>
             <li>
                 <img src="../assets/logo-football.png" alt="">
                </li>
             <li>
              </li>
             <li>
                <font-awesome-icon :icon="facebookIcon" />
            </li>
            <li>
                <font-awesome-icon :icon="instagramIcon" />
            </li>
            <li class="pe-4">
                <font-awesome-icon :icon="twitterIcon" />
            </li>
            </ul>
        </div>
    <div class="">
      <ul class="d-flex justify-content-between gap-3 align-items-center ">

        <li  v-for="(menuItem, index) in menuItems" :key="index" class="text-white">
          <a :href="menuItem.link">{{ menuItem.text }}</a>
        </li>
       
      </ul>
    </div>
  </header>
</template>

<script>
import AppHeaderDinamico from './AppHeaderDinamico.vue'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
import { faFacebook } from '@fortawesome/free-brands-svg-icons'
import { faInstagram } from '@fortawesome/free-brands-svg-icons'
import { faTwitter } from '@fortawesome/free-brands-svg-icons'

export default {
  components: {
    AppHeaderDinamico,
    FontAwesomeIcon
  },
  data() {
    return {
      facebookIcon: faFacebook,
      instagramIcon: faInstagram,
      twitterIcon: faTwitter,
      menuItems: [
        { text: 'HOME', link: '#' },
        { text: 'FIXTURES & RESULTS', link: '#' },
        { text: 'LEAGUE TABLE', link: '#' },
        { text: 'PLAYERS', link: '#' },
        { text: 'GALLERY', link: '#' },
        { text: 'BLOG', link: '#' },
        { text: 'CONTACT', link: '#' }
      ]
    }
  }
}
</script>

<style>
header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000; 
  background-color: rgba(0, 0, 0, 0.2); 
}


header ul {
  list-style: none;
  margin: 0;
  padding: 0;
}

header ul li {
  display: inline-block;
  color: white;
}


</style>
