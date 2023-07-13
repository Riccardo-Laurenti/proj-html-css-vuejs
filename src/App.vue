<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';

  export default {
   
    components: { AppHeader, AppMain, AppFooter,}
};
</script>

<template>
  <div class="container_chess">
    <AppHeader />
    <AppMain />
    <AppFooter />
  </div>
  
 

</template>

<style lang="scss">
  @import "../node_modules/bootstrap/scss/bootstrap";


  .container_chess{
    width: 100%;
    height: 100%;
    margin:auto;
  }
</style>
