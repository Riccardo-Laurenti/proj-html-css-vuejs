<script>
import AppFooterLeft from './Footer/AppFooterLeft.vue'


export default {
  data() {
    return {
        FirstArr:[
            {
                undertitle: 'ZEMEZ ',
                secondtitle: '© ALL RIGHT RESERVED',
                thirdtitle: 'PRIVACY POLICY',
                fourtitle: 'TERMS OF USE'
            },
        ],

    }
  },  
  components: { 
    AppFooterLeft, 
    //AppFooterCentral,
    //AppFooterRight, 
    },
}
</script>

<template>
<section class="section_footer">
    <div class="container " style="color: white">
        <div>
            <AppFooterLeft 
                v-for="index in FirstArr" 
                :key="index.undertitle"
                :undertitle="index.undertitle"
                :secondtitle="index.secondtitle"
                :thirdtitle="index.thirdtitle"
                :fourtitle="index.fourtitle"
            />
        </div>  

            
    </div>


    
</section>
   
  
</template>


<style lang="scss" scoped>

    .button_nav{
        
    } 

    .section_footer{
        background-color: rgb(28, 28, 28);
        height: px;
        padding-top: 7px;
    }
    .container{

        
    }

    .footer{
        
        padding-top: 3.5rem ;
    }
    
    
</style>