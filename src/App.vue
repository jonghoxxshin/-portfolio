<template>
  <div id="app">
    <h1 id="title" v-on:click="titleClick">Jongho Shin</h1>
    <div id="options">
      <ul>
        <div class="row-sm-4">
          <label class="directory" id="homeButton" v-on:click="clicked = 0">Home</label>
          <label class="directory" id="aboutButton" v-on:click="clicked = 1">About</label>
          <label class="directory" id="projectsButton" v-on:click="clicked = 2">Projects</label>
          <label class="directory" id="contactButton" v-on:click="clicked = 3" >Contact</label>
          <label class="directory" id="TodolistButton" v-on:click="clicked = 4">Todo-List</label>
        </div>
      </ul>
    </div>
    <StartView v-if="clicked === 0"/>
    <AboutView v-if="clicked === 1"/>
    <ProjectsView v-if="clicked === 2"/>
    <ContactView v-if="clicked ===3"/>
    <TodolistView v-if="clicked===4"/>
  </div>
</template>

<script>

import StartView from './pages/Start.vue';
import AboutView from './pages/About.vue';
import ProjectsView from './pages/Projects.vue';
import ContactView from './pages/Contact.vue';
import TodolistView from './pages/Todolist.vue';

export default {
  name: 'app',
  components: {
    StartView,
    AboutView,
    ProjectsView,
    ContactView,
    TodolistView
  },
  data () {
    return {
      clicked: 4
    }
  },
  methods: {
    titleClick() {
      let clickedP = document.createElement("p"),
          title = document.getElementById("title");

      clickedP.innerHTML = "hahaha";
      clickedP.onclick = ev => {
        ev.target.remove();
      }

      title.parentElement.insertBefore(clickedP, title.nextSibling);
    }
  }
}



</script>

<style>

  #title{
    font-size: 30pt;

  }

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
  .directory{
    font-size: 24pt;
    color : black;

  }
  ul{
    word-spacing: 30pt;
  }




</style>
