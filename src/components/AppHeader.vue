<template>
    <header class="p-3 text-light">
        <div>
            <ul class="d-flex justify-content-center">
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
                <a href="#"><img src="../../assets/sponsor1.png" alt="">logo</a>
                </li>
            </ul>
        </div>

        <div class="px-5 pt-2">
            <ul class="d-flex justify-content-between">
                 <li>
                     <a href="#">HOME</a>
                    </li>
                 <li>
                     <a href="#">FIXTURES & RESULTS</a>
                    </li>
                 <li>
                     <a href="#">LEAGUE TABLE</a>
                    </li>
                 <li>
                    <a href="#">PLAYERS</a>
                    </li>
                 <li>
                    <a href="#">GALLERY</a>
                    </li>
                    <li>
                    <a href="#">BLOG</a>
                    </li>
                    <li>
                    <a href="#">CONTACT</a>
                    </li>
                    
                </ul>

        </div>

        <section>
            
        </section>
    </header>
</template>
  
  <script>
  
  import { store } from '../store'

  
  export default {
    name: 'AppHeader',
    data() {
      return {
        store
      }
    }
  }
  </script>
  
  <style lang="scss" scoped>
 header{
    background-color: black;
    opacity: 0.7;
    li{
        list-style-type: none;
        a{
            text-decoration: none;
            color: white;
        }
    }
    
 }
  </style>
  
