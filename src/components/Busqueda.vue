<template>
  <div class="hello">
    <h1>Ofertes de Borsa de Treball</h1>

        <b-button @click="oferta" variant="primary">Veure Ofertes</b-button>
        <b-button @click="ordenar" variant="outline-primary">Més Recent</b-button>
    
    
    <hr>
    
    <b-row>
      <b-card-group deck>
        <Ofertes v-for="ofertes in resultado"
            :key="ofertes.id"
            :infoOferta=ofertes>
        </Ofertes>
      </b-card-group>
    </b-row>
        
      
  </div>

  
</template>

<script>

import Ofertes from './Ofertes.vue'

export default {
  name: 'Busqueda',
  data: function(){
    return{
      resultado: []
      
    }
    
  },
  props: {

  },
  components: {
    Ofertes
  },
  methods: {
    oferta: function(){
      this.axios.get('http://labs.iam.cat/~a18jorcuearr/Borsa/api.php/records/oferta').then((response) =>{
        this.resultado=response.data.records;
      })
    },
    ordenar: function(){
      this.resultado.sort(function(a, b){return a.data_pub - b.data_pub})
    }

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

</style>
