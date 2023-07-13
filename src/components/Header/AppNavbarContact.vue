<script>
export default {
    props:{
        write: String
    }
    
}
</script>

<template>
    <div class="d-flex">
            <span class="write">{{ write }}</span>
    </div>
</template>

<style>

    .write{ 
        font-size: 15px;
    }
    
</style>
