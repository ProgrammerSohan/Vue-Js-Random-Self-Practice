<template>
    <div class="event">
        <button @click="handleClick">Event2</button>
        <hr>
        <h4 id="header2">Event Handling2</h4>
    </div>
</template>
<script>
export default {
    name: 'EventHandling',
    methods:{
    handleClick(){
        const header = document.getElementById('header2');
        header.style.color = 'green';
        header.style.fontSize = '50px';
    }
}

}
</script>
<style>
    
</style>