<template>
    <main>
        <!-- sezione world class fitness -->
        <section class="w-class-fit text-center bcg-lightgrey"> 
            <div class="container-xl"> 
                <div class="row">             
                    <h2>WORLD CLASS Fitness</h2>
                    <div>
                        <img class="img-wcf" src="@/assets/divider-xx-red.png" alt="">  
                    </div>                    
                    <p class="paragraph-wcf p-light-gray">At Avada Gym, everything we do from top to bottom is of the highest quality to ensure we’re equipped to help you reach your goals of a healthy and fit lifestyle.</p>
                </div>  
                <div class="divider-candy"></div>              
            </div> 
        </section>

        <!-- sezione form richiesta allenamento di prova gratuito -->
        <section class="form-container bcg-lightblack">            
            <div class="container-xl"> 
                <div class="row">
                    <div class="col-6 img-contenent text-center">
                        <img class="img-form" src="@/assets/home_img-compressor.jpg" alt="">
                    </div>
                    
                    <form class="col-6 form-item">
                        <h3 class="text-light fw-bold mb-5">Sign Up For A Free Training Session</h3>                            
                        <div class="mb-5">
                            <p class="p-light-gray">Name* </p>
                            <input type="text" class="form-control bcg-lightgrey border border-light py-3">
                        </div>                        
                        <div class="mb-5">
                            <p class="p-light-gray">Email</p>
                            <input type="text" class="form-control bcg-lightgrey border border-light py-3" >
                        </div>                        
                        <button><a href="#" class="btn-form button-xlarge bcg-btn-orange text_nounderline text-uppercase text-light">start now</a></button>      
                    </form>
                </div>
            </div>         
        </section>

        <!-- sezione fusion -->
        <section class="fusion bcg-lightblack">            
            <div class="container-xl"> 
                <div class="row">
                    <div class="col-3 img-contenent text-center">                        
                        <i class="fas fa-unlink i-red"></i>
                        <h2 class="text-light fw-bold mb-2">Strength e Conditioning</h2>                                               
                        <img class="img-fusion mb-2" src="@/assets/divider-x-red.png" alt="">
                        <p class="p-light-gray">Lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us.</p>

                    </div>  
                    <div class="col-3 img-contenent text-center">
                        <div>
                            <i class="fas fa-bicycle i-red"></i>
                        </div>                        
                        <h2 class="text-light  fw-bold">Fitness e Cardio</h2>
                        <img class="img-fusion" src="@/assets/divider-x-red.png" alt="">
                        <p class="p-light-gray">Lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us.</p>

                    </div> <div class="col-3 img-contenent text-center">
                        <div>
                            <i class="fab fa-cloudversify i-red"></i>
                        </div>                        
                        <h2 class="text-light  fw-bold">Flexibility e Rest</h2>
                        <img class="img-fusion" src="@/assets/divider-x-red.png" alt="">
                        <p class="p-light-gray">Lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us.</p>

                    </div> <div class="col-3 img-contenent text-center">
                        <div>
                            <i class="fas fa-heartbeat i-red"></i>
                        </div>                        
                        <h2 class="text-light  fw-bold">Health e Diet</h2>
                        <img class="img-fusion" src="@/assets/divider-x-red.png" alt="">
                        <p class="p-light-gray">Lorem ipsum dolor sit amet, consectetur adipiscing elit. In augue nisl, ornare es volutpat etra us.</p>

                    </div>                   
                    
                </div>
            </div>         
        </section>
    </main>
</template>

<script>
export default {
    name: 'Main',   
    
}
</script>

<style scoped lang="scss">
@import '@/style/commons.scss';
main{
    .w-class-fit{
        padding-top: 140px;
        padding-left: 30px;
        padding-right: 30px;
        padding-bottom: 110px;

        h2{
            line-height: 1.28;
            font-size: 2.5rem;
            font-weight: bold;
            color: white;
        }

        .img-wcf{
            width: 30px;
            margin: 30px 0;            
        }

        .paragraph-wcf{
            margin-bottom: 20px;
            padding: 0 175px;
            font-size: 1.25rem;            
        }

        .divider-candy{
            position: relative;
            left: 48.5%;
            bottom: -137px;
            background-color:#25292b;
            height: 55px;
            width: 55px;
            transform: rotate(-45deg);
            border-bottom: 1px solid #25292b;
            border-left: 1px solid #25292b; 
        }
    }

    .form-container {      
        padding-left: 30px;
        padding-right: 30px;
        padding-top: 140px;
        padding-bottom: 70px;

        .img-contenent{ 
            padding: 0 25px;          
            .img-form{
                width: 100%;
                &:hover{                    
                    transform: scale(1.05); // da migliorare leffetto
                    box-shadow: 0 3px 15px rgba(0,0,0,.4);
                }
            }            
        }

        .form-item{
            padding: 0 25px;
            margin-bottom: 20px;
            padding: 0 15px;
            
            .form-control.active{
                background-color: #25292b                
            }
            
            .btn-form{
                width: 100px;
            }
        }

        



        
    }

    .fusion{
        background-image: url('../assets/gym_bkgd_bw-compressor.jpg');
        background-size: cover;
        background-position: center;
        padding-top: 140px;
        padding-left: 30px;
        padding-right: 30px;
        padding-bottom: 110px;

        .img-contenent{
            &:hover{
                color:#ee6059;
            }           

            h2{
                font-size: 1.2rem;
                line-height: 1.28;
                font-weight: bold;
                color: white;
            }

        }

        
        
        

        

    }


}
</style>