<script setup>
const icons = [
  { link: 'https://www.linkedin.com/in/luc%C3%ADa-bermejo/', name: 'fab fa-linkedin', text: 'Linkedin Lucia Bermejo' },
  { link: 'https://github.com/lubersol', name: 'fab fa-github', text: 'Github Lubersol' },
  { link: 'https://drive.google.com/file/d/1TwAf8TBNe90bmmgfx-3isSyFnGSZwDyo/view?usp=sharing', name: 'fa-solid fa-file', text: 'CV Lucia Bermejo' },
]
</script>

<template>
  <div class="home-hero__socials">
    <div v-for="(icon, index) in icons" :key="index" class="home-hero__social">
      <a :href="icon.link" class="home-hero__social-icon-link" rel="noreferrer" target="_blank">
        <i :class="icon.name" style="font-size:x-large; color:black; width:100%" :alt="icon.text"></i>
      </a>
    </div>
  </div>
</template>

