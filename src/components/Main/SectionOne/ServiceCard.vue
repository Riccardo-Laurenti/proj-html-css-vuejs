<script>
export default {
    props: {
        image: String,
        text:  String,
        title: String,
        description: String,
        seconddescription: String,
    } 
}
</script>


<template>
    <div class="sub_col">
        <div class="item_service" style="padding-top: 124px;">

            <h1 style="font-size: 40px; font-weight: 900; line-height: 24px;">{{ text }}</h1>

            <div class="d-flex" style="margin-top: 20px; margin-bottom: 20px;">
               <hr style="width: 20%; ; border: 1px solid rgb(0, 159, 252)">
               <hr style=" width: 70%; color: grey; border: 1px solid grey" > 
            </div>
            
            <h6 style="font-weight: 600; margin-bottom: 40px; line-height: 24px;">{{ title }}</h6>
            <p class="p_main" style="margin-bottom: 40px; line-height: 24px;">{{ description }}</p> 
            <p class="p_two_main" style="line-height: 24px; margin-bottom: 30px;">{{ seconddescription }}</p>

        </div>
        
    </div>
</template>



<style>

    .item_service h1  {
        margin-top: 90px;
        margin-bottom:20px;
    }
    
</style>