<template>
    <header class="jumbo"> 
        <div class="headernav"> 
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
        </div>

        
              
            <div class="text-jumbo text-center text-light">
                <div class="row">
                    <div class="col">
                        <h1 class="text-uppercase fw-bold">no pain no gain</h1>
                        <h2>Motivation is what gets you started. Habit is what keeps you going.</h2>
                        <div class="btn-jumbo">
                            <button class="bcg-btn-trasparent" ><a href="https://avada.theme-fusion.com/gym/membership/" class="text_nounderline text-uppercase">join us today</a></button>
                        </div>
                    </div>
                    
                    


                </div> 
            </div>  
        
        
                       
         
        
        
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
@import '@/style/commons.scss';

.jumbo{
    background-image: url('../assets/home-banner.jpg');
    background-size: cover;
    height: 580px;

    .headernav{
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
   

    
    
    
    .text-jumbo{
        h1{
            font-size: 7rem;                      
            line-height: 1;          
        }

        h2{
            font-size: 1.25rem;             
            letter-spacing: 1px;  
            margin-top: 30px;   
            margin-bottom: 20px;    
        }

        .btn-jumbo{
            a{
                color: #b8b9b9; 
                &:hover{
                        color: white;
                }
            }
        }
    }    
}




    



</style>