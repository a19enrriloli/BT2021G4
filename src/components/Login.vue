<template>
  <div id="head">
    
    <b-container >
       <b-row class="justify-content-md-center">
           <b-button @click="login" size="sm" variant="success">Inicia Sessió</b-button>
         
       </b-row>
    </b-container>
  </div>
</template>

<script>

export default {
  name: 'Login',
  ddata: function(){
    return {
  
    }   
  },
  components: {
      //login: function(){
      //}
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
}
</style>