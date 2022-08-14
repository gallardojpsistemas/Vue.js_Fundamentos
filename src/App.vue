<script>
  export default{
    data: () => ({
      contador:10,
    }),
    methods: {
      saludar(){
        console.log("Hola estoy saludando");
      },
    }
  };
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="Logo Vue" width="125" height="125">
    <small>
      <h1>Template es una etiqueta HTML, permite ejecutar adentro codigo html</h1>
    </small>
    <hr />
    <h2>Contador: {{contador}}</h2>
    <button v-on:click="saludar()">+1</button>
    <button>-1</button>
    <button>Reset</button>
  </div>
</template>

<style scoped>
  .container{
    text-align: center;
    background-color: #dddd;
  }

  small{
    color: #666;
  }

  h1{
    font-weight: bolder;
  }

  h2{
    font-size: 2.5rem;
  }

  button{
    cursor: pointer;
    font-size: 1.5rem;
    margin: 0px 6px;
  }
</style>