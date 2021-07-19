<template>
    <header class="">        
        <section class="headernav">
            <div class="row">
                <div class="col-3 logo-contenent">
                    <a class="" href="https://avada.theme-fusion.com/gym/membership/"><img src="@/assets/gym_logo_1x.png" alt=""></a>

                </div>

                <nav class="col-6 navbar text-light">                    
                    <ul class="">
                        <li v-for="(link,index) in links" :key="index"><a href="#" class="text-uppercase" > {{link.text}} </a></li>                            
                    </ul>                
                </nav> 

                <div class="col-3 joinusitem d-flex justify-content-end">
                    <button class="bcg-btn-orange" ><a href="https://avada.theme-fusion.com/gym/membership/" class="text_nounderline text-uppercase text-light">join us today!</a></button>

                </div>
            </div>

            
        </section> 
        
       <section class="jumbo">
            
       </section> 
    </header>
</template>

<script>
export default {
  name: 'Header', 

  data() {
    return {
      links: [          

        {
            text : 'Home',
        }, 
        {
            text : 'About us',
        }, 
        {
            text : 'Facilities',
        },
        {
            text : 'Membership',
        }, 
        {
            text : 'Testimonial',
        }, 
        {
            text : 'Blog',
        },  
      ]
    }
  }
}
</script>

<style scoped lang="scss">

.headernav{
    background-color: black;
    padding: 30px 70px;

    ul{  
        margin-top: 12px;

        li{       
            display: inline-block;
            margin-right: 45px;        
            font-size: 1.25rem;        
        
            a{
                color: white;
                text-decoration: none;

                
                &:hover{
                    color: #ee6059;
                }
            }    
                
        }
    }

    

    .joinusitem{
        padding: 40px 0;
    }

    
}

    



</style>