<template>
    <section class="sfondo">
      <div class=" p-4 text-light d-flex gap-3 justify-content-between align-items-center text-start">

        <div>
            <ul class="">
                <li class="my-3"><img src="../assets/logo-footer-football.png"  alt=""></li>
                <li class="my-3 d-flex align-items-center gap-1">
                    <font-awesome-icon :icon="locationDotIcon" class="fa-2x pe-3"/>
                <h4 class="mt-1">New Jersey, USA</h4></li>
                <li class="my-3 d-flex align-items-center gap-1">        <font-awesome-icon :icon="phoneVolumeIcon" class="fa-2x pe-2"/>

                <h4 class="mt-1"> +1 (234) 567 89 10</h4></li>
                <li class="my-3 d-flex align-items-center gap-1">    <font-awesome-icon :icon="envelopeIcon" class="fa-2x pe-2" />
                <h4 class="mt-1">example@example.com</h4></li>
                <ul class="d-flex gap-4 my-4">
            <li class="icona px-3 py-1">
                <font-awesome-icon :icon="facebookIcon" class="fa-2x" />
            </li>
            <li class="icona px-3 py-1">
                <font-awesome-icon :icon="instagramIcon" class="fa-2x" />
            </li>
            <li class="pe-4 icona px-3 py-1">
                <font-awesome-icon :icon="twitterIcon" class="fa-2x" />
            </li>
                </ul>
            </ul>
        </div>
    
        <div>
            <h2 class="fw-4 my-3">Join Our Newsletter</h2>
            <p>Subscrivr to be informed about important <BR></BR>developments in oour club and football world.</p>

            <div class="input-group input-group-lg w-70">
  
                <input type="text" class="form-control" aria-label="Sizing example input" aria-describedby="inputGroup-sizing-lg"
                placeholder="Your mail address">
            </div>
            <button type="button" class="btn btn-light  w-100
            mt-2 p-3">Subscribe</button>
        </div>
        
        <div class="d-flex flex-column align-items-center">
            <h2>Educacion</h2>
            <ul>
                <li   v-for="(menuItem, index) in menuItems" :key="index" >
                  <font-awesome-icon :icon="faMinus" />
                <a  class="text-white px-1" :href="menuItem.link">{{ menuItem.text }}</a>
        </li>
            </ul>
        </div >
        <div class="d-flex flex-column align-items-start">
            <h2>Quick Links</h2>
            <ul>
                <li v-for="(menuItemdue, index) in menuItemsdue" :key="index">
                  <font-awesome-icon :icon="faMinus" />
                 <a class="text-white px-1" :href="menuItemdue.link">{{ menuItemdue.text }}</a>
                </li>
            </ul>
        </div>
    <div>      
</div> 
      </div>
<div class="d-flex justify-content-center text-white">
  <p class=" ">
    2022 Football Club - All Rights Reserved.
  </p>
</div>
</section>

</template>
      
<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { faFacebook } from '@fortawesome/free-brands-svg-icons';
import { faInstagram } from '@fortawesome/free-brands-svg-icons';
import { faTwitter } from '@fortawesome/free-brands-svg-icons';
import { faLocationDot, faPhoneVolume, faEnvelope } from '@fortawesome/free-solid-svg-icons';
import AppFooterDinamico from './AppFooterDinamico.vue';
import { faMinus } from '@fortawesome/free-solid-svg-icons';


export default {
  components: {
    FontAwesomeIcon,
    AppFooterDinamico
    
  },
  name: 'AppFooter',
  data() {
    return {
      facebookIcon: faFacebook,
      instagramIcon: faInstagram,
      twitterIcon: faTwitter,
      locationDotIcon: faLocationDot,
      phoneVolumeIcon: faPhoneVolume,
      envelopeIcon: faEnvelope,
      faMinus: faMinus,
      menuItems: [
        { text: 'FIXTURES & RESULTS', link: '#' },
        { text: 'LEAGUE TABLE', link: '#' },
        { text: 'PLAYERS', link: '#' },
        { text: 'GALLERY', link: '#' },
      ],
      menuItemsdue: [
        { text: 'HOME', link: '#' },
        { text: 'BLOG', link: '#' },
        { text: 'GALLERY', link: '#' },
        { text: 'CONTACT', link: '#' },
      ]
    };
  }
};
</script>
      
      <style lang="scss" scoped>
      img{
        width: 50px;
      }
      .icona{
        border: 1px solid white;
      }
      .sfondo{
        background-image: url("../assets/footer-bg-football.jpg");
      }
      </style>
      
    