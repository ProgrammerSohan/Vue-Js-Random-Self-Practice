<template>
    <div class="event">
        <button @click="toggleHeader">Toggle Event</button> <hr>
        <h5 id="toghead">Event Toggle</h5>
    </div>
</template>
<script>
export default {
    name: 'EventHandling',
    data(){
        return {
            isToggled: false, //state to track toggle status
        };
    },
    methods: {
        toggleHeader(){
            const header = document.getElementById('toghead');

            if(this.isToggled){
                //reset to original state
                header.style.color = 'black';
                header.style.fontSize = '16px';
            }else{
                header.style.color = 'green';
                header.style.fontSize = '50px';
            }
            this.isToggled = !this.isToggled;
        }

    }

    
}
</script>
<style>
    
</style>