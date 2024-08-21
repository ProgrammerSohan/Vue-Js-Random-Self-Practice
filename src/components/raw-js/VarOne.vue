<template >
    <div>
        <h1>Javascript Variable in Vue.js</h1>
        <p>In this example, x,y & z are declared within vue.js data properties.</p>
        <p>The value of Z is: {{ z }}</p>
        
    </div>
</template>
<script>
export default {
    data(){
        return{
            x: 5,
            y: 61,
        };
    },
    computed: {
        z(){
            return this.x + this.y;
        }
    }
    
}
</script>
<style >
    
</style>