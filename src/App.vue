<script>
  export default{
    data:() => ({
      contador: 10,
    }),
    methods: {
      incrementar(){
        // contador = contador + 1;
        this.contador++;
      },
      decrementar(){
        this.contador--;
      },
      reset(){
        this.contador = 10;
      },
    }
  };
</script>

<template>
 <!-- <div class="alert alert-success text-center fixed-top " role="alert">
  <h4 class="alert-heading">C1-S1</h4>
  <p>Isabel Cristina Simón Morales</p>
  <hr>
  <p class="mb-0">10° "A" DGS</p>
</div> -->


 <!-- <div class="mtop"> -->
 <img src="./assets/logo.svg"  alt="logo" width="125" height="125">
  <div class="container mtop">
    <h1> Hola desde VUE.js 3  </h1> <hr>
  <h2>
    Contador {{contador}}
  </h2>
  <!-- @ === v-on: -->
  <button @click="incrementar()">+1</button>
 
  <button @click="decrementar">-1</button>
  <button @click="reset">Reset</button>
  </div>
 

 <!-- </div> -->
  
</template>

<style scoped>

  h1{
  font-weight: bolder;
    /* color:red; */
  }
  .container{
  text-align: center;
  }
  .mbo{
    margin-bottom: 155px;
  }

  small{
    color:#666;
  }

  h2{
    font-size: 2.5rem;
  }
  button{
    cursor:pointer;
    font-size: 1.5 rem;
    margin: 0px 8px;

  }
  
</style>

