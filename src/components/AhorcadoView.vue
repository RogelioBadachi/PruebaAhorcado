
<template>
<!-- CSS only -->

  <div class="container">
    <div class="cuadroMono">
      <div class="monito">
        <img src="../assets/ahorcado.png" class="img-fluid" alt="...">
      </div>
      <div class="letters">
        {{letters}}
      </div>
      
    </div>
    <div class="letras">
      
    </div>
    <div class="escritura">
      <b-form-textarea
        id="textarea"
        v-model="text"
        placeholder="Enter something..."
        rows="3"
        max-rows="6"
      ></b-form-textarea> 
      <h3 class="holi" ref="holi">{{holi}}</h3>
      <button class="ingresarLetras" @click="formatting">Ingresar</button>
      <button type="button" class="btn btn-primary">Primary</button>
      <div class="input-group mb-3">
        <button class="btn btn-outline-secondary" @click="hola" type="button" id="button-addon1">Button Hola</button>
        <input type="text" class="form-control" v-model="inputData" placeholder="Ingrese letra por letra" aria-label="Example text with button addon" aria-describedby="button-addon1">
      </div>
    </div>
    
  </div>
</template>

<script>

export default {
  data() { 
    return{
      text: "",
      holi: "",
      inputData: "",


    }
  },
  name: 'AhorcadoView',
  props: {
    msg: String
  },

  methods:{
    formatting: function(){
      this.holi = "holi";
    },
    hola: function(){
      this.holi = this.inputData;
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
  height: 20rem;
  width: 15rem;
  border: solid 10px black;
  position: relative;
  top: 50%;
  left: 40%;
}

</style>
