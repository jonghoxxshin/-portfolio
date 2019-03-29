<template>
    <div id="About">

      <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
        <!-- Bootstrap CSS -->
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
        <title>About</title>
      </head>

      <body>

      <p>
        Jongho Shin is a student at Duke University studying Computer Science and Political Science
      </p>
        <div class="row-sm-4">
          <img src="../assets/laughingattrees.jpg" width="400" height="400" alt="profile">
        </div>

      </body>
    </div>
</template>

<script>
    export default {
        name: "About",
      data(){
          return{

          }
      },

    }
</script>

<style scoped>

  #About {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  title, p{
    font-weight: normal;
    font-size: 15pt;
    text-align: center;

  }
  p:hover {
    color: dimgray;
  }
  img{
    align: center;
  }
</style>
