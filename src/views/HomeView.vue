<script setup>
import ButtonItem from '@/components/ButtonItem.vue'
import SocialMediaItem from '@/components/SocialMediaItem.vue'

const icons = [
  {
    id: 1,
    name: 'fab fa-linkedin',
    link: 'https://www.linkedin.com/in/luc%C3%ADa-bermejo/',
    text: 'Linkedin Lucia Bermejo'
  },
  {
    id: 2,
    name: 'fab fa-github',
    link: 'https://github.com/lubersol',
    text: 'Github Lubersol'
  },
  {
    id: 3,
    name: 'fa-solid fa-file',
    link: 'https://drive.google.com/file/d/1kBPe6RL3Vn-fe6zkrT69YsUX1lyXZwZV/view?usp=sharing',
    text: 'CV Lucia Bermejo'
  }
]
</script>

<template>
  <div class="home-hero">
    <div class="home-hero__content">
      <h1 class="heading-primary">Hey, I'm Lucía Bermejo</h1>
      <div class="home-hero__info">
        <p class="text-primary">
          A Fullstack focused Web Developer building the Frontend of Websites
          and Web Applications that leads to the success of the overall
          product
        </p>
      </div>
      <ButtonItem text="Projects" href="/projects" />
    </div>  
  </div>
  <SocialMediaItem :icons="icons" />
</template>

<style>
.home-hero {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
  margin: 0;
  color: #fff;
  background: linear-gradient(to right,rgba(245,245,245,.8),rgba(245,245,245,.8)),url('/subtle-prism.svg');
  background-position: center;
  height: 100vh;
  min-height: 80rem;
  max-height: 120rem;
  position: relative;
}
.home-hero__content {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  max-width: 90rem;
  width: 92%
}
.heading-primary {
  font-size: 5rem;
  text-transform: uppercase;
  letter-spacing: 3px;
  text-align: center;
  color: #111;
  font-weight: 800;
}
.home-hero__info {
    margin: 3rem auto 0 auto;
    max-width: 80rem;
}
.text-primary {
    color: #333;
    font-size: 2rem;
    text-align: center;
    width: 100%;
    line-height: 1.6;
}

@media only screen and (max-width: 37.5em) {
  .home-hero {
    height: unset;
    min-height: unset;
  }
  .home-hero__content {
    padding: 19rem 0 13rem 0;
    margin: auto;
    position: static;
    transform: translate(0,0);
  }
  .heading-primary {
    font-size: 4rem;
  }
  .text-primary {
    font-size: 2rem;
  }
}

</style>