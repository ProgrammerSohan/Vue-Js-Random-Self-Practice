<template>
   <div>
    <GeteventData />
   </div>
  </template>
   <script>
  //import Class from './components/Class.vue'
  import GeteventData from './components/GeteventData.vue';

  
  export default{
    name: 'App',
    data(){
       return {
         test: 'Sohan1111'
       }
    },
    components: { 
      //Class,
        GeteventData
    }
  
  }
   
   </script>
   <style>
   #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
 
  
   </style>