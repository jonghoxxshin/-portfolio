<template>
  <!--<head>-->
    <!--<meta charset="utf-8">-->
    <!--<meta name="viewport" content="width=device-width,initial-scale=1">-->
    <!--<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">-->
    <!--<title>Projects</title>-->
  <!--</head>-->
  <div id="body">
    <div class="container">
      <div class="row center">
        <div class="card-body">
          <hr>
          <a class="project_name">Music Chat Live</a>
          <a href="http://musicchat.live" class="card-title">(Link)</a>
          <p class="card-text">Messenger Application that allows users to listen to same music simultaneously while chatting.</p>
          <hr>
        </div>
        <div class="row center">
          <div class="col-md-12 card">
            <img src="../assets/music_chat_front.b479365.png" class="card-img-top">
          </div>
          <div class="col-md-12 card">
            <img src="../assets/music_chat_chat.d55f8b1.png" class="card-img-top">
          </div>
        </div>
      </div>
      <div class="row center">
        <div class="card-body">
          <hr>
          <a class="project_name">NFL Breakout!</a>
          <p class="card-text">Variation of Atari's Breakout. Play to win the SuperBowl!</p>
          <hr>
        </div>
        <div class="row center">
          <div class="col-md-12 card">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/E58-oyDhF6c" frameborder="0"
                    allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          </div>
        </div>
      </div>
      <div class="row center">
        <div class="card-body">
          <hr>
          <a class="project_name">Cell Society Simulation</a>
          <p class="card-text">Cellular automata models</p>
          <hr>
        </div>
        <div class="row center">
          <div class="col-md-12 card">
            <iframe width="560" height="315" src="https://www.youtube.com/embed/twklzOWy3nY" frameborder="0"
                    allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
          </div>
        </div>
      </div>

    </div>
  </div>

    
</template>

<script>
    export default {
        name: "Projects"
    }
</script>

<style scoped>
  .project_name{
    font-weight: bold;
    font-size: large;
  }
</style>
