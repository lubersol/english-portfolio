<script setup>
import TitleItem from '../components/TitleItem.vue'
import ProjectItem from '../components/ProjectItem.vue'

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
