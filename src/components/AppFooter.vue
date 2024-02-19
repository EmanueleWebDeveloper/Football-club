<template>
    <section class="bg-black p-4 text-light d-flex gap-3 justify-content-between align-items-center text-start">
        <div>
            <ul>
                <li class="my-3"><img src="../assets/logo-footer-football.png"  alt=""></li>
                <li class="my-3"><h4>New Jersey, USA</h4></li>
                <li class="my-3"><h4> +1 (234) 567 89 10</h4></li>
                <li class="my-3"><h4>example@example.com</h4></li>
                <ul class="d-flex gap-4 my-4">
                    <li>icona</li>
                    <li>icona</li>
                    <li>icona</li>
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
            mt-2 p-3">Large button</button>
        </div>
        
        <div>
            <h2>Educacion</h2>
            <ul>
                <li class="my-2">- FIXTURES & RESULTS</li>
                <li>- LEAGUE TABLE</li>
                <li class="my-2">- PLAYERS</li>
                <li>- GALLERY</li>
            </ul>
        </div>
        <div>
            <h2>Educacion</h2>
            <ul>
                <li class="my-2">- FIXTURES & RESULTS</li>
                <li>- LEAGUE TABLE</li>
                <li class="my-2">- PLAYERS</li>
                <li>- GALLERY</li>
            </ul>
        </div>
        
        <div>
        
        </div> 


    </section>
</template>
      
      <script>
      
      import { store } from '../store'
    
      
      export default {
        name: 'AppFooter',
        data() {
          return {
            store
          }
        }
      }
      </script>
      
      <style lang="scss" scoped>
      img{
        width: 50px;
      }
      </style>
      
    