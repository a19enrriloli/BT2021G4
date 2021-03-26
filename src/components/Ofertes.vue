<template>
  <div>
    <b-card :title=infoOferta.titol >
        <b-card-text>

            <p>{{infoOferta.descripcio}}</p>
            <p>{{infoOferta.ubi}}</p>
            <p>{{infoOferta.data_pub}}</p>

        </b-card-text>
    </b-card>

  </div>
  
</template>

<script>
export default {
  name: 'Ofertes',
  data: function(){
      return {

      }
  },
  props: {
    infoOferta: {}
  },
  methods: {

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
