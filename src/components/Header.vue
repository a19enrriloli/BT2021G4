<template>
  <div id="head">
    
    <b-container >
       <b-row class="justify-content-md-center">
         <Login/>
        <Empresa/>
        <Admin/>
         
       </b-row>
    </b-container>
  </div>
</template>

<script>
import Empresa from './Empresa.vue'
import Admin from './Admin.vue'
import Login from './Login.vue'

export default {
  name: 'Header',
  ddata: function(){
    return {
  
    }   
  },
  components: {
      Empresa, Admin, Login
  }
}
</script>

<style>
#head {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  padding: 5px; 
}
</style>
