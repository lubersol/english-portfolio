<script setup>
import { RouterView } from 'vue-router'
import MenuRow from './components/MenuRow.vue';
import LogoItem from './components/LogoItem.vue';
</script>

<template>
  <header class="header">
    <div class="header__content">
      <LogoItem />
      <MenuRow />
    </div>
  </header>

  <RouterView />
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
</style>
