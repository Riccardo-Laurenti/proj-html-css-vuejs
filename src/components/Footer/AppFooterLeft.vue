<script>
export default {
    props:{
        undertitle: String,
        secondtitle: String,
        thirdtitle: String,
        fourtitle: String,
    }
}
</script>


<template>


            <div class="d-flex  justify-content-between align-items-center">  
                <div>
                    <span style="font-size: 13px; ">{{ undertitle }}  </span> 

                    <span style="font-size: 13px; color: rgb(187, 185, 185);" >{{ secondtitle }}  </span> 

                    <span style="padding-left: 18px; padding-right: 18px; ">|</span>

                    <span style="font-size: 13px;">{{ thirdtitle }} </span> 

                    <span style="padding-left: 18px; padding-right: 18px; ">|</span>

                    <span style="font-size: 13px;">{{ fourtitle }} </span> 
                </div>

                <div>
                    <span class="task-item"><a href="#"><i class="fa-brands fa-facebook-f fa-sm my-c"></i></a></span>
                    <span class="task-item" style="margin-left: 18px; margin-right: 18px;"><a href="#"><i class="fa-brands fa-twitter fa-sm my-c"></i></a></span>
                    <span class="task-item"><a href="#"><i class="fa-brands fa-instagram fa-sm my-c"></i></a></span>
                    
                </div>
            </div>
</template>


<style lang="scss" scoped>
.my-c {
  color: black;
}

.task-item {
    border-radius: 50%;
    width: 19px;
    height: 19px;
    display: inline-block;
    font-size: 14px;
    vertical-align: middle;
    text-align: center;
    //line-height: 15px;
    background: grey;
}
</style>
