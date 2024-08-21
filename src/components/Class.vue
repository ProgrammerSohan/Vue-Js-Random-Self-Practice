<template>
    <div class="test2"> Class </div>
    <div>{{sohan}}</div>
</template>
<script>
export default {
    name: 'Class',
    props:{
        sohan: String,
    }
}
</script>
<style>
.test2{
    background:green;
}
    
</style>