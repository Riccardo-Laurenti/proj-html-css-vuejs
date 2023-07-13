<script>
import AppNavbar from './Header/AppNavbar.vue';
import AppNavbarContact from './Header/AppNavbarContact.vue';
import AppNavJumbo from './Header/AppNavJumbo.vue';

export default {
components:{
    AppNavbar,
    AppNavbarContact,
    AppNavJumbo,
},
data() {
        return {
            FirstArrayHarder: [
                {
                    write:'7087 Richmond hwy, Alexandria, VA',
                },
                
            ],
            SecondArrayHarder: [
                {
                    write:'800-2345-6789',
                }
            ],

            ArrayHarder: [
                
                {
                    title: 'HOME',
                },
                {
                    title: 'SERVICES',
                },
                {
                    title: 'YACHTS',
                },
                {
                    title: 'RESERVATIONS',
                },
                {
                    title: 'BLOG',
                },
                {
                    title: 'CONTACTS',
                },
                
            ],
            HeaderJumbo: [
                
                {
                    title: 'QuickWind',
                    text: 'all kinds of boats, yacht charters and sailing destinations for hobbyist yachtsmen and women!',
                },
                
            ],
        };
    },
}
</script>

<template>
    <section class="section_header">
        <div class="container_header">
            <section class="section_nav">
                <div class="d-flex flex-column" >
                    <div class="first_navbar d-flex flex-row align-items-center" style="">
                        
                        <div class="d-flex flex-row justify-content-center align-items-center" style="width: 72%;">
                            <div class="d-flex align-items-center">
                            <i class="fa-solid fa-location-dot px-2"></i>
                            <AppNavbarContact
                            v-for="element in FirstArrayHarder" 
                            :key="element.write"
                            :write="element.write"
                            />
                            <i class="fa-solid fa-location-dot px-2" style="margin-left: 60px"></i>
                            <AppNavbarContact
                            v-for="element in SecondArrayHarder" 
                            :key="element.write"
                            :write="element.write"
                            />
                            </div>
                        </div>
                        
                        
                        <div class=" div_button d-flex justify-content-center" style="font-size: 15px; flex-basis: 58%;">
                           <span class="task-item">  <i class="fa-brands my-white fa-facebook-f"></i>  </span>
                           <span class="task-item" style="margin-left:18px;margin-right:18px;">  <i class="fa-brands my-white fa-twitter"></i>  </span>
                           <span class="task-item">  <i class="fa-brands my-white fa-instagram"></i>  </span>
                        </div>  
                    </div>
                    
                    <div class="navbar d-flex justify-content-center align-items-center" style="color:white; font-weight: 400;"> 
                        <div style="flex-basis: 21%;"><img src="./../assets/quickwind/images/logo.png" alt="" class="logo img-fluid" style="height: 81px;"></div>   
                        
                        <div class="d-flex flex-row" style="flex-basis: 50%; font-weight: 900;">
                            <AppNavbar 
                            v-for="index in ArrayHarder" 
                            :key="index.title"
                            :title="index.title"
                            /> 
                        </div>
                        <div><i class="fa-solid fa-location-dot fa-magnifying-glass"></i></div>
                    </div>
                </div>
            </section>
        
            <section class="section_title">
              
                <div class="container_title d-flex flex-column" style="; color:white;">
                  <div class="mb-3"
                        style="font-size: px; padding-top: 130px;"> 
                                <AppNavJumbo 
                                v-for="index in HeaderJumbo" 
                                :key="index.title"
                                :title="index.title"
                                :text="index.text"
                                /> 
                  </div>

                    
                
                    <div class="mt-4">
                        

                        <button 
                        class=" button_nav py-2 rounded-1" 
                        style="border: 1px solid white; background-color: transparent; color:white; font-weight: 900;">
                            Learn More
                        </button>
                    </div>
                </div>
            </section>   
        </div>   
    </section>    
</template>


<style lang="scss">

    .task-item {
        border-radius: 50%;
        width: 26px;
        height: 24px;
        display: inline-block;
        /* font-size: 14px; */
        vertical-align: middle;
        text-align: center;
        background: grey;
    }


    .my-white {
        color: white;
    }





    .fa-location-dot{
        color: #18beff;  
    }

    .section_header{
        background-image: url(./../assets/quickwind/images/bg1-1.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        height: 65rem;
    }

    
    .section_nav{
        height: 9rem;
        color: white;
    }



    .first_navbar{
        height: 52px;
        background: #e7e7e7;
        width: 100%;
        padding: 5px;
        color: #030303;
    }

    .div_button{
        padding-left:9.2rem
    }
    
    .button_nav{
        padding-inline: 2rem;
    }






    .section_title{
        height: 84%;
        width: 55%;
        margin: auto;
        padding-top: 7rem;
    }

   

    .container_title{
        position: relative;
        padding-right:2rem;
    }

    
    

    .first_button_nav{
        padding-inline: 0.7rem;
    }

    .button_nav{
        padding-inline: 2.4rem;
        transition: transform 0.2s;
        &:hover{
            transform: scale(0.95);
        }
    }

</style>