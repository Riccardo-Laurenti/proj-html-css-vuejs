<script>
export default {
    props:{
        title: String,
    }   
};
</script>

<template>
    <div class="list_component">{{ title }}</div>
</template>


<style lang="scss">
    .sub_navbar{
        width: 100%;
    }

    .list_component{
        padding-inline: 1.6rem;
    }

    .list_component:hover{
        color: lightblue;
        cursor: pointer;
    }
</style>