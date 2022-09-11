<script>
  export default{
    data:() => ({
      contador: 500,
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
 <div class="alert alert-success text-center fixed-top " role="alert">
  <p>Isabel Cristina Simón Morales</p>
  <hr>
  <p class="mb-0">10° "A" DGS</p>
</div>


 <img src="./assets/logo.svg"  alt="logo" width="125" height="125" class="mtC">
  <div class="container mtC">
    <h1> Hola desde VUE.js 3  </h1> <hr>
  <h2>
    Contador {{contador}}
  </h2>
  <!-- @ === v-on: -->
  <button @click="incrementar()">+1</button>
 
  <button @click="decrementar">-1</button>
  <button @click="reset">Reset</button>
  </div>
  
</template>

<style scoped>
  .mtC{
    margin-top: 150px;
  }
  h1{
  font-weight: bolder;
    /* color:red; */
  }
  .container{
  text-align: center;
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

