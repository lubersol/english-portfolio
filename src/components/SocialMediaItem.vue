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

<style scoped>
.home-hero__socials {
  position: absolute;
  top: 35%;
  transform: translateY(-50%);
  background: #fff;
  box-shadow: rgba(100,100,111,.2) 0 7px 29px 0;
  padding: .5rem;
}
.home-hero__social {
  width: 5rem;
}
.home-hero__social-icon-link {
    width: 100%;
    display: block;
    padding: 1rem;
    /* transition: background .3s; */
    border-radius: 5px;
}
.home-hero__social-icon-link:hover {
    background: rgba(120,67,233,.2);
}

@media only screen and (max-width: 56.25em) {
  .home-hero__socials {
    display: none;
  }
}
</style>
