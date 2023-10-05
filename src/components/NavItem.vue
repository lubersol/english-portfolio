<script setup>
import { RouterLink } from 'vue-router'
import { computed, ref  } from 'vue'

const links = [
  { text: 'Home', to: '/' },
  { text: 'About', to: '/about' },
  { text: 'Projects', to: '/projects' },
  { text: 'Contact', to: '/contact' },
]

const showDropdown = ref(false)

const toggleDropdown = () => {
  showDropdown.value = !showDropdown.value;
}

const iconClass = computed(() => {
  return showDropdown.value ? 'fa fa-times' : 'fa fa-bars'; // Clases CSS de los iconos
})
</script>

<template>
  <!-- Horizontal navigation -->
  <div class="header__main">
    <ul class="header__links">
      <li v-for="(link, index) in links" :key="index" class="header__link-wrapper">
        <RouterLink :to="link.to" class="header__link">{{ link.text }}</RouterLink>
      </li>
    </ul>
    <div class="header__main-ham-menu-cont" @click="toggleDropdown">
      <i :class="iconClass" class="header__main-ham-menu"></i>
    </div>  
  </div>
  <!-- Dropdown menu -->
  <div v-if="showDropdown" class="header__sm-menu header__sm-menu--active">
    <div class="header__sm-menu-content">
      <ul class="header__sm-menu-links">
        <li v-for="(link, index) in links" :key="index" class="header__sm-menu-link">
          <RouterLink :to="link.to" @click="toggleDropdown">{{ link.text }}</RouterLink>
        </li>
      </ul>
    </div>
  </div>
</template>

<style>
.header__links {
  display: flex;
}
.header__link {
  padding: 2.2rem 3rem;
  display: inline-block;
  font-size: 1.6rem;
  color: #333;
  text-transform: uppercase;
  letter-spacing: 1px;
  font-weight: 700;
  transition: color .3s;
}
ul a.router-link-exact-active {
  color: #7843e9;
}
ul a.header__link:hover {
  color: #7843e9;
}
.header__main-ham-menu {
  width: 100%;
  font-size: x-large;
  cursor: pointer;
  transition: 0.8s ease all;
}
.header__main-ham-menu-cont {
  display: none;
  width: 3rem;
  padding: 2.2rem 0;
}
.header__main-ham-menu-cont-active {
  transform: rotate(180deg);
}
.header__sm-menu {
  background:#fff;
  position:absolute;
  width:100%;
  top:100%;
  visibility:hidden; 
  opacity:0; 
  transition:all .3s;
  box-shadow:0 5px 5px 0 rgba(0,0,0,.1);
  -webkit-box-shadow:0 5px 5px 0 rgba(0,0,0,.1);
  -moz-box-shadow:0 5px 5px 0 rgba(0,0,0,.1);
}  
.header__sm-menu--active {
  visibility:visible; 
  opacity:1;
}
.header__sm-menu-link a {
  display:block;
  text-decoration:none;
  padding:2.5rem 3rem;
  font-size:1.6rem;
  color:#333;
  text-align:right;
  border-bottom:1px solid #eee;
  font-weight:700;
  text-transform:uppercase;
  letter-spacing:2px;
  transition:color .3s;
}
.header__sm-menu-link a:hover {
  color:#7843e9;
}
.header__sm-menu-link:first-child a {
  border-top:1px solid #eee;
}
.header__sm-menu-link-last {
  border-bottom:0;
}  
@media only screen and (max-width:37.5em) {
  .header__links {
    display:none;
  }
  .header__main-ham-menu-cont {
    display:block;
  }
  .header__sm-menu--active {
    visibility: visible;
    opacity: 1;
  }
}
@media only screen and (max-width:56.25em) {
  .header__link{
    padding:3rem 1.8rem;
    font-size:1.5rem;
  }
} 

</style>
