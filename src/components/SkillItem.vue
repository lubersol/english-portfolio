<script setup>

const skills = [
  { text: 'HTML' },
  { text: 'CSS' },
  { text: 'JavaScript' },
  { text: 'React' },
  { text: 'VUE' },
  { text: 'Pinia' },
  { text: 'Jest' },
  { text: 'GIT' },
  { text: 'Github' },
  { text: 'NodeJS' },
  { text: 'Express' },
  { text: 'PHP' },
  { text: 'Laravel' },
  { text: 'SQL' },
  { text: 'MongoDB' },
  { text: 'Terminal' },
  { text: 'Responsive Design' },
  { text: 'SEO' },
  { text: 'SASS' },
]
</script>

<template>
  <div class="about__content-skills">
    <h3 class="about__content-title">My Skills</h3>
    <div class="skills">
      <div v-for="(skill, index) in skills" :key="index" class="skills__skill">{{ skill.text }}</div>
    </div>
  </div>  
</template>

<style>
.about__content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-gap: 10rem;
}
.skills {
  display:flex;
  flex-wrap:wrap;
}
.skills__skill {
  padding:1rem 2rem;
  margin-bottom:1.5rem;
  margin-right:1.5rem;
  font-size:1.6rem;
  background:rgba(153,153,153,.2);
  border-radius:5px;
  font-weight:600;
  color:#666;
}

@media only screen and (max-width: 56.25em) {
  .about__content {
    grid-template-columns: 1fr;
    grid-gap: 8rem;
  }
}
</style>