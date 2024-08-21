<template>
    <div>
        <button @click="handleClick(11111)">Click for parameters to event</button>
    </div>
</template>
<script>
export default {
    name: 'Para2Event',
    methods: {
        handleClick(sohan){
            console.log('PARAM',sohan);
        },

    },
    props:{
        msg: String,
    }
    
}
</script>
<style>
    
</style>