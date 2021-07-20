<template>
    <footer class="">
        
        <section class="footer-up bcg-lightgrey">
            <div class="container-xl"> 
                <div class="row">
                    <div class="col-9">
                        <div class="row">
                            <div class="col-4"></div>
                            <div class="col-4"></div>
                            <div class="col-4"></div>
                        </div>                       
                    </div>
                    <div class="col-3 d-flex">
                        
                    </div>
                </div>
            </div>
        </section>

        <section class="footer-down bcg-lightblack">
            <div class="container-xl">
                <div class="row">
                    <div class="col-9 footer-down-text">
                        <p class="text-light-gray">© Copyright 2015 | Avada Theme by <a href="https://theme-fusion.com/">ThemeFusion</a> | All Rights Reserved | Powered by <a href="http://wordpress.org">WordPress</a></p>   
                    </div>
                    <div class="col-3 d-flex footer-down-icon">
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
    data(){
        return{
            
        }
    },    
}
</script>

<style scoped lang="scss">
@import '@/style/commons.scss';
.footer-up{
    height: 420px;
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