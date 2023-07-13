<script>
export default {
    props: {
        title: String,
        text:  String,
    } 
}
</script>

<template>
    <div class="nav-jumbo">
            <h1>{{ title }}</h1>
            <p>{{ text }}</p>
    </div>
</template>

<style>
    .nav-jumbo h1 { 
        font-size: 106px;
        font-weight: 900;
    }

    .nav-jumbo p { 
        font-size: 32px;
        font-weight: 900;
        width: 97%;
        letter-spacing: 3px;
    }
</style>