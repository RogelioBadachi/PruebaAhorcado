
<template>
<!-- CSS only -->

  <div class="home">
    <div class="cuadroMono">
      <div class="monito">
        
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
      <h3 class="holi" ref="holi">jiji {{holi}}</h3>
      <button class="ingresarLetras" @click="formatting">Ingresar</button>
      <button type="button" class="btn btn-primary">Primary</button>
      <div class="input-group mb-3">
      <button class="btn btn-outline-secondary" @click="holi" type="button" id="button-addon1">Button</button>
        <input type="text" class="form-control" placeholder="" aria-label="Example text with button addon" aria-describedby="button-addon1">
      </div>
    </div>
    
  </div>
</template>

<script>

export default {
  data() { 
    return{
      text: "",
      holi: ""

    }
  },
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
