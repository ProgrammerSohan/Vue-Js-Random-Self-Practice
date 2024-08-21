<template>
    <div class="hello">Hello Sohan 01</div>
    <div>Hello Vue JS3</div>
    <div>{{msg}}</div>
    <div>
        <h3>{{name}}</h3>
        <h3>{{ age }}</h3>
        <h3>{{gender}}</h3>
        <h3>{{ "My Name Is Sohan" }}</h3>

        <br> <br> <hr>
        <div v-bind:id="myId">Attribute Binding Here01: {{myId}}</div>
        <hr>
        <img :src="mySrc" alt="" width="350" height="350" />
        <hr>
        <h2 :class="myH2">Dreamer Sohan!</h2>
        <br> <hr>
        <!-- <button v-on:click="handleClick">Click</button> -->
         <button @click="handleClick">Click</button>
        <h1 id="header">Event Handling</h1>

    </div>
</template>
<script>
export default {
    name: 'HelloSohan',
    methods:{
        handleClick(){
            const header = document.getElementById('header');
            header.style.color = 'blue';
        }
    },
    data(){
        return{
            name: 'Sohan Ami',
            age: 29,
            gender: true,
            myId: 'divId',
            mySrc: '../watch.png',
            myH2: 'myH2',
        };
    },
    props:{
        msg: String,
    }
    
}
</script>
<style scoped>
    
.hello{
    background: orange;
}
#divId{
    background: yellow;
}
.myH2{
    background: orangered;
}

</style>