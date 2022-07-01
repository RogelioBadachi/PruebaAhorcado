<template>
  <div class="home">
    <div class="cuadroMono">
      <div class="monito">
        <h3 class="holi" ref="holi">{{holi}}</h3>
      </div>
    </div>
    <div class="letras">

    </div>
    <div class="escritura">
      <button class="ingresarLetras" @click="formatting">Ingresar</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AhorcadoView',
  props: {
    msg: String
  },

  methods:{
    formatting: function(){
      this.holi = "holi";
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
.cuadroMono {
  height: 300px;
  width: 200px;
  border: solid 10px black;
}
</style>
