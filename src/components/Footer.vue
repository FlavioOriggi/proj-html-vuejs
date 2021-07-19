<template>
    <footer class="">
        
        <section class="footer-up bcg-lightgrey">
            <div class="container-lg"> 
                <div class="row">
                    <div class="col-3"></div>
                    <div class="col-3"></div>
                    <div class="col-3"></div>
                    <div class="col-3"></div>
                </div>
            </div>
        </section>

        <section class="footer-down bcg-lightblack text-light">
            <div class="container-lg">
                <div class="row d-flex">
                    <div class="col-6">bla</div>
                    <div class="col-6">opla</div>
                    
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
    height: 115px;
}



</style>