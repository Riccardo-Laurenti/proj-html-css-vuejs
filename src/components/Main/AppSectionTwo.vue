<script>
export default {

}
</script>



<template>
    <section class="second-section" style="background-color: #FFCD18;">
        <div class="prova">
         <h1>Yacht Charters, Repairs <br> & Transportation, US-wide!</h1>
         <button class=" button_nav py-2 rounded-1 me-3 border-0" style="color:white; font-weight: 600; background-color: #16a9bd;">
                           More Details
                        </button>
        </div>

    </section>
</template>



<style lang="scss" scoped>
    .second-section {
        background-color: rgb(255, 205, 24);
        color: white;
        height: 800px;
        background-image: url(./../../assets/quickwind/images/bg5.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }

    .prova {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 800px;
        flex-direction: column
    }
    .prova h1 {
        font-weight: 900;
        line-height: 118px;
        font-size: 93px;
        text-align: center;
        margin-bottom: 50px;
    }
    
</style>