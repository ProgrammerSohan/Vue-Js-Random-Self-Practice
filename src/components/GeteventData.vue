<template>
    <div>
        <h3>Get Event Data</h3>
        <button @click="getData">Click for Event Data</button>
    </div>
</template>
<script>
export default {
    name: 'GeteventData',
    methods:{
        getData(event){
            const {target} = event;
            console.log(event);
            target.style.backgroundColor = 'green';
        }

    }
    /*,
    props:{
        msg: String,
    }*/
   
}
</script>
<style>
    
</style>