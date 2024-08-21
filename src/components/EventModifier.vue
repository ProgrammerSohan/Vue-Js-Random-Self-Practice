<template>
    <div>
       <!--  <form @submit="handleSubmit"> -->
        <form @submit.prevent="handleSubmit">
            <label for="">Event Modifier</label><br>
            <input type="text"> <br>
            <button type="submit">Submit</button>

        </form>

        <button @click="onBtnClick">Inc</button> 
        <!-- <button @click.once="onBtnClick">Inc</button> -->
            <p>{{ number }}</p>
    </div>
</template>
<script>
export default {
    name: "EventModifier",
    methods: {
        handleSubmit(){//e
           // e.preventDefault();
            console.log("Form Submitted");
        },
        onBtnClick(){
            this.number=this.number + 1
        }
    },
    data(){
       // return{};
       return {
          number: 1,
       };
    },
    props: {
        msg: String,
    }
    
}
</script>
<style>
    
</style>