<template>
  <header :class="{ 'scrolled': scrolled }" class="p-3 text-light fixed-top">
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
             <li class="icona">
                <font-awesome-icon :icon="facebookIcon" class="fa-2x" />
            </li>
            <li>
                <font-awesome-icon :icon="instagramIcon" class="fa-2x" />
            </li>
            <li class="pe-4">
                <font-awesome-icon :icon="twitterIcon" class="fa-2x" />
            </li>
            </ul>
        </div>
    <nav class="responsive">
      <ul class="d-flex justify-content-between align-items-center pt-4">

        <li   v-for="(menuItem, index) in menuItems" :key="index" >
          <a class="text-white px-1 mx-5" :href="menuItem.link">{{ menuItem.text }}</a>
        </li>
       
      </ul>
    </nav>
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
      scrolled: false,
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
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      
      this.scrolled = window.scrollY > 490; 
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
li a:hover {
  border-bottom: 2px solid white;
}
header.scrolled {
  transform: translateY(-100%);
  transition: transform 0.3s ease-in-out;
}


</style>
