<template>
  <div id="Todolist">

    <head>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
      <!-- Bootstrap CSS -->
      <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
      <title>Todolist</title>
    </head>


    <body>
    <div class="row mx-4">
      <input class="col-md-4 mx-md-auto my-md-4" type="text" id="myInput" placeholder="What do you have to do?" v-on:keypress.enter="addInput()"/>
    </div>
    <div class="row mx-4">
      <button class="col-md-4 mx-md-auto my-md-4" type="button" id="myBtn" v-on:click="addInput()">Add</button>
    </div>
    <div class="row mx-4">
      <ul class="col-md-4 mx-md-auto" id="todo">

      </ul>
    </div>

    </body>
  </div>
    
</template>

<script>
    export default {
        name: "Todolist",
      methods:{
          addInput() {
            let tmp = document.getElementById("myInput"),
                list = document.getElementById("todo");
            let add = document.createElement("p");
            add.innerText = tmp.value;
            list.appendChild(add);
            tmp.value = "";
            add.onclick = ev => ev.target.remove();
          }

      }
    }

</script>

<style scoped>

  #Todolist{
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  #todo {
    border: solid 1pt black;
  }

  #myInput{
    color: black;
    border: solid 1pt black;
  }

  p {
    word-spacing: normal;
  }


  h1{
    font-weight: normal;
  }


</style>
