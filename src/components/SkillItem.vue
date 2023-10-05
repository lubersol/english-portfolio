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

