<template>
    <header class="jumbo" id="startpage">

        <!-- sezione header + navbar   -->
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
        
        <!-- sezione jumbo   -->
        <div class="text-jumbo text-center">
            <div class="header-icon-display-right">
                <div class="contenent-icon-display-header mb-2">
                    <i class="fas fa-folder"></i>
                    <p>Demon</p>
                </div>
                <div class="contenent-icon-display-header">
                    <i class="fas fa-folder"></i>
                    <p>Buy Now</p>
                </div>
            </div>
            <div class="row text-light">
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
    height: 100vh;

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
        .header-icon-display-right{
            position: absolute;
            position: fixed;
            right: 7px;
            z-index: 9999;

            .contenent-icon-display-header{
                background-color: white;
                height: 60px;
                width: 60px;
                padding: 6px;
                border-radius: 5px; 
                color: #33475b;
                &:hover{
                    cursor: pointer;
                }               
                p{
                    font-size: 0.75rem;
                }            
            }

        }
         

        h1{
            font-size: 7rem;                      
            line-height: 1;   
            margin-top: 10%;       
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