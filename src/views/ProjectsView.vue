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

