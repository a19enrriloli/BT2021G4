<template>
  <div id="head">
    
    <b-container >
       <b-row class="justify-content-md-center">
           <b-button @click="empresa" size="sm" variant="info">Ets empresa?</b-button>
         
       </b-row>
    </b-container>
  </div>
</template>

<script>

export default {
  name: 'Empresa',
  ddata: function(){
    return {
  
    }   
  },
  components: {
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