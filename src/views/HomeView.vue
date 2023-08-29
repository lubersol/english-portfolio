<script setup>
import ButtonItem from '../components/ButtonItem.vue';
import MenuColumn from '../components/MenuColumn.vue';
</script>

<template>
  <div class="home-hero">
    <MenuColumn />
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
</template>

<style>
.home-hero {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
  margin: 0;
  color: #fff;
  /* background-image: url('/subtle-prism.svg'); */
  background: linear-gradient(to right,rgba(245,245,245,.8),rgba(245,245,245,.8)),url('/subtle-prism.svg');
  /* background: linear-gradient(to right,rgba(245,245,245,.8),rgba(245,245,245,.8)),url(https://d33wubrfki0l68.cloudfront.net/daac8858fd4a0ccea44f59dfd079c3c16c263f33/c157c/assets/svg/common-bg.svg); */
  background-position: center;
  height: 100vh;
  min-height: 80rem;
  max-height: 120rem;
  position: relative;
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
/* .home-hero__social-menu {
  display: flex;
  align-self: flex-start;
} */
.text-primary {
    color: #333;
    font-size: 2rem;
    text-align: center;
    width: 100%;
    line-height: 1.6;
}
@media (min-width: 1024px) {
  .home-hero {
    min-height: 100vh;
    display: flex;
    align-items: center;
  } 
}
</style>