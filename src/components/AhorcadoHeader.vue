
<template>
<!-- CSS only -->

  <h1>Ahorcado</h1>
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
  name: 'AhorcadoHeader',
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
h1 {
  color:black;
  font-family: 'Dancing Script', cursive;
  font-size: 4rem;
}

</style>
