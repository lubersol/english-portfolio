<script setup>
import { RouterView } from 'vue-router'
import LogoItem from './components/LogoItem.vue'
import NavItem from './components/NavItem.vue'
import FooterItem from './components/FooterItem.vue'

</script>

<template>
  <header class="header">
    <div class="header__content">
      <LogoItem />
      <NavItem />
    </div>
  </header>
  <RouterView />
  <footer class="main-footer">
    <FooterItem />
  </footer>
  
</template>

<style scoped>
.main-footer {
  background:#000;
  color:#fff;
}
</style>
