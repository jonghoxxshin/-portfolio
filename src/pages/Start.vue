<template>
  <div id="Start">

    <head>
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

      <!-- Bootstrap CSS -->
      <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">

      <title></title>

    </head>

    <body>

      <img src="../assets/background.jpg" height="800" width="1000">
      <hr>
    </body>
  </div>
</template>

<script>
    export default {
        name: "Start",
      data() {
          return {

          }
      }
    }
</script>

<style scoped>
  #Start {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  .cool-a {
    font-size: 24pt;
    color: black;
    text-decoration: none !important;
  }

  .cool-a:hover {
    color: gray;
  }

  #options {
    display: inline;
    word-spacing: 50px;
  }

  .b1:hover{
    color: gainsboro;
  }
  h1, h2 {
    font-weight: normal;
  }

  img {
    width: 100%;
    height: 100%;
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

  label {
    font-size: 30px;
  }

  @media screen and (max-width: 376px) {
    h1 {
      font-size: 36pt;
    }

    label {
      font-size: 20px;
    }
  }
</style>
