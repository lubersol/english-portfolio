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
.header {
  position: fixed;
  width: 100%;
  z-index: 1000;
  background: #fff;
  box-shadow: 0 10px 100px rgba(0,0,0,.1);
}
.header__content {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 5rem;
}
.main-footer{
    background:#000;
    color:#fff;
}
@media only screen and (max-width:56.25em) {
    .header__content{
        padding:0 2rem;
    }
}
</style>
