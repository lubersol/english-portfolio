<script setup>

const projects = [
  { picture: '/vp.png', title: 'Varitx Paradise', text: 'App created with React in the Front-end and with Laravel (PHP) in the Back-end. It is like an agrotourism website where you can make reservations to spend a stay in Mallorca. You can do register and login, and select dates, type of room and there is a photo gallery too.' },
  { picture: '/filmsskl.png', title: 'Films SKL', text: 'Rest API created with React in the Front-end part and Laravel (PHP) in the Back-end part. It consists of an audiovisual content platform (movies) where you can watch streaming movies. You can do register and login, and see a popular movies page too.' },
  { picture: '/dental.png', title: 'Dental clinic', text: 'App created with React on the front-end and with NodeJS and Express on the back-end. It is an application that simulates a dental clinic website where you can make appointments and delete them.' },
  { picture: '/witcher.png', title: 'The witcher', text: 'Simulation of a fighting video game created with HTML5, CSS3 and JS. It consists of a home screen with a "Play" button to go to the screen with 4 players. Choose 2 players and press the "Fight" button to start the game.' },
  { picture: '/comecocos.png', title: 'Pac-man', text: 'Pac-man video game console created with HTML5, CSS3 and JS. When you press the central button on the console, the central image changes to a black screen, simulating an on/off button; and a transition effect on the central screen that when you position yourself with the mouse changes the image simulating movement in the screen.' },
  { picture: '/lubersolfilms.png', title: 'Lubersol films', text: 'Rest API created with React on the Front-end and MovieDB API. The user can register in the application, do log in/logout, access their customer area, process a movie rental from the browser and search for movies by title.' },
]

</script>

<template>
  <div v-for="(project, index) in projects" :key="index" class="projects__row">
    <div class="projects__row-img-cont">
      <img :src="project.picture" alt="Project Screenshot" class="projects__row-img"
        loading="lazy" />
    </div>
    <div class="projects__row-content">
      <h3 class="projects__row-content-title">{{ project.title }}</h3>
      <p class="projects__row-content-desc">{{ project.text }}</p>
    </div>
  </div>
</template>

