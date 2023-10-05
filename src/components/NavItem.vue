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


