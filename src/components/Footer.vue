<template>
    <footer class="">
        
        <!-- sezione parte superiore -->
        <section class="footer-up bcg-lightgrey">
            <div class="footer-icon-display-right">
                <div class="contenent-icon-display-footer text-light text-center">
                    <a class="text-light text_nounderline" href="#startpage"><i class="fas fa-chevron-up"></i></a>
                </div>
            </div>
            <div class="container-xl"> 
                <div class="row">
                    <div class="col-9">
                        <div class="row">
                            <div class="col-4">                                
                                <div class="text-footer-up-contenent" >
                                    <h4 class="text-uppercase text-middle-gray">come find us</h4>
                                    <div v-for="(element,index) in comefindus" :key="index">
                                        <p class="text-light-gray mt-5">{{element.text}}</p>
                                        <div class="text-light-gray my-2">Phone: <span class="text-footer-up-color">{{element.numberphone}}</span></div>
                                        <div class="text-light-gray">Email: <span class="text-footer-up-color">{{element.emailaddres}}</span></div>

                                    </div>
                                </div>                                
                            </div>
                            <div class="col-4">
                                <div class="text-footer-up-contenent recent-posts-space">                                    
                                    <h4 class="text-uppercase text-middle-gray ">recent posts</h4>
                                    <div v-for="(element,index) in recentposts" :key="index">
                                        <div class="border-list-recentposts"> <span class="text-footer-up-color me-2" ><i class="fas fa-chevron-right"></i></span><a class="text-footer-up-color text_nounderline" href="https://avada.theme-fusion.com/gym/2015/05/12/should-you-lift-free-weights-or-just-your-body-weight/">{{element.text}}</a></div>                                            
                                    </div>                                    
                                </div>
                            </div>
                            <div class="col-4">
                                <div class="text-footer-up-contenent">                                    
                                    <h4 class="text-uppercase text-middle-gray ">opening times</h4>
                                    <div class="" v-for="(element,index) in openingtimes" :key="index">
                                        <div class="text-light-gray mt-5">{{element.text}}</div>
                                        <div class="text-middle-gray mt-2">{{element.hour}}</div>
                                    </div>                                    
                                </div>
                            </div>
                        </div>                       
                    </div>
                    <div class="col-3 footer-up-img p-3">
                        <img class="card-img" src="@/assets/gym_ad-compressor.jpg" alt="https://avada.theme-fusion.com/gym/membership/">                        
                    </div>
                </div>
            </div>
        </section>

        <!-- sezione parte inferiore  -->
        <section class="footer-down bcg-lightblack">
            <div class="container-xl">
                <div class="row">
                    <div class="col-9 footer-down-text">
                        <p class="text-light-gray">© Copyright 2015 | Avada Theme by <a href="https://theme-fusion.com/">ThemeFusion</a> | All Rights Reserved | Powered by <a href="http://wordpress.org">WordPress</a></p>   
                    </div>
                    <div class="col-3 d-flex justify-content-end footer-down-icon">
                        <div class="footer-icons facebook-icons"><i class="fab fa-facebook-f"></i></div>
                        <div class="footer-icons twitter-icons"><i class="fab fa-twitter"></i></div>
                        <div class="footer-icons insta-icons"><i class="fab fa-instagram"></i></div>
                        <div class="footer-icons youtube-icons"><i class="fab fa-youtube"></i></div>   
                    </div>                    
                </div>
            </div>            
        </section> 
    </footer>   
</template>

<script>
export default {
name: 'Footer',
data() {
    return {
        comefindus: [
            {
                text : '12345 North Main Street New York, NY 555555',
                numberphone : '1.800.555.6789',
                emailaddres : 'info@your-domain.com'
            }        
        ],
        recentposts: [
            {
                text : 'Train with free weights or your body weight?',
            }, 
            {
                text : 'Nutritional advice that will keep you training',
            } 
        ],
        openingtimes: [
            {
                text : 'Weekdays Monday – Friday',
                hour : '09:00 – 19:00'
            }, 
            {
                text : 'Weekends Saturday – Sunday',
                hour : '09:00 – 21:00'
            }
        ]
    }
  }
}
</script>

<style scoped lang="scss">
@import '@/style/commons.scss';
.footer-up{
    padding: 85px 30px 85px 30px;

    .footer-icon-display-right{
        position: absolute;
        right: 5%;  
        bottom: 0; 
        position: fixed;     
        z-index: 99;

        .contenent-icon-display-footer{
            height: 35px;
            width: 50px;
            background-color: #303030;
            border-top-left-radius: 5px;
            border-top-right-radius: 5px;
            &:hover{                    
                background-color: #ee6059;                            
                cursor: pointer;                       
            }        
        }
    }

    .text-footer-up-contenent{
        padding-right: 35px;

        .text-footer-up-color{
            color: white;
            &:hover{                    
                color: #ee6059;                            
                cursor: pointer;                       
            }
        }       
    }
    .recent-posts-space{
        h4{
            margin-bottom: 33px;
        }          
        .border-list-recentposts{
            border-bottom: 1px solid #3e3e3e;
            width: 100%;
            padding: 15px 0;
        }
    }   

    .footer-up-img{
        img{
            &:hover{                    
                transform: scale(1.05);
                transition: 0.5s;
                box-shadow: 0 3px 15px rgba(0,0,0,.4);
                cursor: pointer;                       
            }
            
        }
    }
}

.footer-down{
    padding: 35px 30px 35px 30px;

    .footer-down-text{
        margin: 15px 0;
        a{
            color: white;
            text-decoration: none;
            &:hover{                    
                color: #ee6059;                            
                cursor: pointer;                       
            }
        }
    }
    .footer-down-icon{
        .facebook-icons{                 
            padding-top: 4px;
            padding-left: 14px;                    
        }
        .twitter-icons, .insta-icons{                   
            padding-top: 5px;
            padding-left: 12px;                      
        }        
        .youtube-icons{        
            padding-top: 5px;
            padding-left: 10px;                   
        }
        .facebook-icons, .twitter-icons, 
        .insta-icons, .youtube-icons{
            &:hover{                    
                opacity: 0.8;                            
                cursor: pointer;                       
            }  
        }
    }    
}


            


    


</style>