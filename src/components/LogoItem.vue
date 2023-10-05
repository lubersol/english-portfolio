<script setup>
import { useRouter } from 'vue-router';

const router = useRouter();
const goHome = () => {
  router.push({ name: 'home' })
}

</script>

<template>
  <div class="header__logo-container" @click="goHome">
    <div class="header__logo-img-cont">
      <img src="/foto_lucia_bermejo.png" alt="Lucia Bermejo Logo Image" class="header__logo-img">
    </div>
    <span class="header__logo-sub">Lucia Bermejo</span>
  </div>
</template>

