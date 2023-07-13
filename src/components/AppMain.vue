<script>
import 'bootstrap/dist/js/bootstrap.min.js';

import AppSectionOne from './Main/AppSectionOne.vue';
import AppSectionTwo from './Main/AppSectionTwo.vue';
import AppSectionThird from './Main/AppSectionThird.vue';
import AppSectionFour from './Main/AppSectionFour.vue';
import AppSectionFive from './Main/AppSectionFive.vue';
import AppSectionSix from './Main/AppSectionSix.vue';




export default {
    components:{
        AppSectionOne,
        AppSectionTwo,
        AppSectionThird,
        AppSectionFour,
        AppSectionFive,  
        AppSectionSix,
    }
}
</script>

<template>
    <AppSectionOne />
    <AppSectionTwo />
    <AppSectionThird />
    <AppSectionFour />
    <AppSectionFive />
    <AppSectionSix />
</template>


<style lang="scss" scoped></style>