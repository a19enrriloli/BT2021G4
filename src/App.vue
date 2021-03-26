<template>
  <div id="app">
    <Header/>
    <img alt="Vue logo" src="./assets/logo.png">
    <b-container >
       <b-row class="justify-content-md-center">

        <Busqueda/>          
         
       </b-row>
    </b-container>
  </div>
</template>

<script>

import Busqueda from './components/Busqueda.vue'
import Header from './components/Header.vue'
export default {
  name: 'App',
  ddata: function(){
    return {
  
    }   
  },
  components: {
    Busqueda, Header
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
