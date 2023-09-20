<script setup>
defineProps({
  projects: {
    type: Array,
  },  
  picture: {
    type: String,
    required: false
  },
  title: {
    type: String,
    required: false
  },
  text: {
    type: String,
    required: false
  }
})
</script>

<template>
  <div v-for="project in projects" :key="project.title" class="projects__row">
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
<style scoped>
.projects__row {
    display: grid;
    grid-template-columns: 1.5fr 1fr;
    grid-gap: 5rem;
    margin-bottom: 11rem;
}

.projects__row-img-cont {
    overflow: hidden;
}
.projects__row-img {
    width: 100%;
    display: block;
    -o-object-fit: cover;
    object-fit: cover;
    border: 0.5px solid gray;
}
.projects__row-content {
    padding: 2rem 0;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: flex-start;
}
.projects__row-content-title {
    font-weight: 700;
    font-size: 2.8rem;
    margin-bottom: 2rem;
}
.projects__row-content-desc {
    font-size: 1.8rem;
    color: #666;
    max-width: 60rem;
    line-height: 1.7;
    margin-bottom: 3rem;
}
</style>