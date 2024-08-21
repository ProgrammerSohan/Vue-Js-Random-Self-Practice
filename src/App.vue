<template>
  <h1 class="test">Testing</h1>
  <Class sohan="This is a variable!!"/>
  <Class2 />
  <HelloSohan msg="Hi, I am Sohan, practicing Vue JS3!!"/>
  <h1>{{ test }}</h1>
  <hr>
  <EventHandling />
</template>
 <script>
import Class from './components/Class.vue'
import Class2 from './components/Class2.vue'
import HelloSohan from './components/HelloSohan.vue';
import EventHandling from './components/EventHandling.vue';
export default{
  name: 'App',
  data(){
     return {
       test: 'Sohan1111'
     }
  },
  components: { 
    Class,
    Class2,
    HelloSohan,
    EventHandling
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
.test{
  background: red;
}

 </style>