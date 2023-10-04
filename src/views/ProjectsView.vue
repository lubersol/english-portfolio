<script setup>
import TitleItem from '../components/TitleItem.vue'
import ProjectItem from '../components/ProjectItem.vue'

const projects = [
  {
    picture: '/vp.png',
    title: 'Varitx Paradise',
    text: 'App created with React in the Front-end and with Laravel (PHP) in the Back-end. It is like an agrotourism website where you can make reservations to spend a stay in Mallorca. You can do register and login, and select dates, type of room and there is a photo gallery too.'
  },
  {
    picture: '/filmsskl.png',
    title: 'Films SKL',
    text: 'Rest API created with React in the Front-end part and Laravel (PHP) in the Back-end part. It consists of an audiovisual content platform (movies) where you can watch streaming movies. You can do register and login, and see a popular movies page too.'
  },
  {
    picture: '/dental.png',
    title: 'Dental clinic',
    text: 'App created with React on the front-end and with NodeJS and Express on the back-end. It is an application that simulates a dental clinic website where you can make appointments and delete them.'
  },
  {
    picture: '/witcher.png',
    title: 'The witcher',
    text: 'Simulation of a fighting video game created with HTML5, CSS3 and JS. It consists of a home screen with a "Play" button to go to the screen with 4 players. Choose 2 players and press the "Fight" button to start the game.'
  },
  {
    picture: '/comecocos.png',
    title: 'Pac-man',
    text: 'Pac-man video game console created with HTML5, CSS3 and JS. When you press the central button on the console, the central image changes to a black screen, simulating an on/off button; and a transition effect on the central screen that when you position yourself with the mouse changes the image simulating movement in the screen.'
  },
  {
    picture: '/lubersolfilms.png',
    title: 'Lubersol films',
    text: 'Rest API created with React on the Front-end and MovieDB API. The user can register in the application, do log in/logout, access their customer area, process a movie rental from the browser and search for movies by title.'
  },
]
</script>

<template>
  <div id="projects" class="projects sec-pad">
    <div class="main-container">
      <TitleItem title="Projects" subtitle text="Here you will find some of the personal and clients projects that I
        created with each project containing its own case study">
      </TitleItem>
      <div class="projects__content">
        <ProjectItem :projects="projects"></ProjectItem>
      </div>
    </div>
  </div>
</template>

<style>
.sec-pad {
    padding: 12rem 0;
}
.main-container {
  max-width: 120rem;
  margin: auto;
  width: 92%;
}
@media only screen and (max-width:56.25em){
  .sec-pad{
      padding:8rem 0;
  }
}

</style>
