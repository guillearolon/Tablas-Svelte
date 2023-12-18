<script>

  let contar = 1;
  
  $: multiplicarUno = contar * 1;
  $: multiplicarDos = contar * 2;
  $: multiplicarTres = contar * 3;
  $: multiplicarCuatro = contar * 4;
  $: multiplicarCinco = contar * 5;
  $: multiplicarSeis = contar * 6;
  $: multiplicarSiete = contar * 7;
  $: multiplicarOcho = contar * 8;
  $: multiplicarNueve = contar * 9;
  $: multiplicarDiez = contar * 10;
  
  
  function multi(){
      contar +=1;
      multiplicarUno;
      multiplicarDos;
      multiplicarTres;
      multiplicarCuatro;
      multiplicarCinco;
      multiplicarSeis;    
      multiplicarSiete;
      multiplicarSiete;
      multiplicarOcho;
      multiplicarNueve;
      multiplicarDiez;
  }
  </script>
  
  <h1>Tabla de multiplicar del {contar}</h1>
  
  <button on:click={multi}>Multiplicar</button>
  
  <div class="contenedor">
      <div class="flex">
          <p>{contar} x 1 = {multiplicarUno}</p>
          <p>{contar} x 2 = {multiplicarDos}</p>
          <p>{contar} x 3 = {multiplicarTres}</p>
          <p>{contar} x 4 = {multiplicarCuatro}</p>
          <p>{contar} x 5 = {multiplicarCinco}</p>
      </div>    
      <div class="flex">
          <p>{contar} x 6 = {multiplicarSeis}</p>
          <p>{contar} x 7 = {multiplicarSiete}</p>
          <p>{contar} x 8 = {multiplicarOcho}</p>
          <p>{contar} x 9 = {multiplicarNueve}</p>
          <p>{contar} x 10 = {multiplicarDiez}</p>
      </div>
  </div>
  
  <style>
      button{
          width: max-content;
          background-color: blueviolet;
          padding: 10px;
          margin-bottom: 10px;
          font-family: monospace;
          font-size: 20px;
          font-weight: bold;
      }
  
      h1{
          text-align: start;
          font-family: monospace;
          font-weight: bold;
          font-size: 30px;
      }
  
      p{
          text-align: center;
          font-family: monospace;
          font-weight: bold;
          font-size: xx-large;
      }
  
      .contenedor{
          display: flex;
          background-color: beige;
          width: max-content;
          border-radius: 5px;
          border-style: groove;
      }
  
      .flex{
          border: 1px solid black;
          border-radius: 10px;
          padding: 12px;
          width: max-content;
          margin: 5px;
      }
  </style>