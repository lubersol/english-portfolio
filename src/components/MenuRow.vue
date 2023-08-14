<script setup>
import { RouterLink } from 'vue-router'

// defineProps({
//   link: {
//     type: String,
//     required: true
//   }
// })
</script>

<template>
  <div class="header__main">
    <ul class="header__links">
      <li class="header__link-wrapper">
        <RouterLink to="/" class="header__link">Home</RouterLink>
      </li>
      <li class="header__link-wrapper">
        <RouterLink to="/about" class="header__link">About</RouterLink>
      </li>
      <li class="header__link-wrapper">
        <RouterLink to="/projects" class="header__link">Projects</RouterLink>
      </li>
      <li class="header__link-wrapper">
        <RouterLink to="/contact" class="header__link">Contact</RouterLink>
      </li>
    </ul>
    <div class="header__main-ham-menu-cont">
      <img src="https://d33wubrfki0l68.cloudfront.net/79e75114856ae61628d2ad26504e3ff4ab2c71b6/f06a4/assets/svg/ham-menu.svg" alt="hamburger menu" class="header__main-ham-menu">
      <img src="https://d33wubrfki0l68.cloudfront.net/de2a681c8ca1630b29949b3a34bf158a686a0554/6a0ec/assets/svg/ham-menu-close.svg" alt="hamburger menu close" class="header__main-ham-menu-close d-none">
    </div>
  </div>
</template>

<style scoped>
ul a.router-link-exact-active {
  color: #7843e9;
}
ul a.header__link:hover {
  color: #7843e9;
}
.header__links {
  display: flex;
}
.header__link {
  padding: 2.2rem 3rem;
  display: inline-block;
  font-size: 1.3rem;
  color: #333;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: 700;
  transition: color .3s;
}
*, ::after, ::before {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
  font-family: inherit;
}
ul {
  display: block;
  list-style-type: disc;
  /* margin-block-start: 1em; */
  /* margin-block-end: 1em; */
  margin-inline-start: 0px;
  margin-inline-end: 0px;
  padding-inline-start: 40px;
}
li {
  list-style: none;
}
.header__main-ham-menu-cont {
  display: none;
  width: 3rem;
  padding: 2.2rem 0;
}
</style>
