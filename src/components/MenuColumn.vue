<script setup>
defineProps({
  title: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="home-hero__socials">
    <div class="home-hero__social">
      <a href="https://www.linkedin.com/in/luc%C3%ADa-bermejo/" class="home-hero__social-icon-link" rel="noreferrer" target="_blank">
        <img src="https://d33wubrfki0l68.cloudfront.net/d8e6e1e636531e28274a1b8b6d947b817f6145bd/d42d3/assets/svg/linkedin-dark.svg" alt="Ram Maheshwari Linkedin Profile" class="home-hero__social-icon">
      </a>
    </div>
    <div class="home-hero__social">
      <a href="https://github.com/lubersol" class="home-hero__social-icon-link" rel="noreferrer" target="_blank">
        <img src="https://d33wubrfki0l68.cloudfront.net/38469cf88d038b6ba3322c9fcb93a8f7167df4b9/cb0b9/assets/svg/github-dark.svg" alt="RammCodes Github Profile" class="home-hero__social-icon">
      </a>
    </div>
    <!-- TODO:INCLUIR AQUÍ ENLACE A MI CV EN GOOGLE DRIVE (en inglés!!!)COMO EN EL OTRO PORTFOLIO -->
    <div class="home-hero__social">
      <a href="https://drive.google.com/file/d/1R90FcVZ2RrA8ydEq9guHF7vDjfAd314-/view" class="home-hero__social-icon-link" rel="noreferrer" target="_blank">
        <img src="https://d33wubrfki0l68.cloudfront.net/e978c8491d93813aa00b3dc80b9abfb0d64a9086/3c187/assets/svg/book-dark.svg" alt="RammCodes DEV.to Blog Profile" class="home-hero__social-icon">
      </a>
    </div>
  </div>
</template>

<style scoped>
.home-hero__socials {
  display: flex; 
  flex-direction: column;
  align-self: flex-start; 
  width: 5.8rem;
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  background: #fff;
  box-shadow: rgba(100,100,111,.2) 0 7px 29px 0;
  padding: 0.5rem;
}
.home-hero__social {
  width: 4rem;
}
</style>
