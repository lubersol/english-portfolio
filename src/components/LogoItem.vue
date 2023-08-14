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

<style scoped>
.header__logo-container {
    display: flex;
    align-items: center;
    cursor: pointer;
    color: #333;
    transition: color .3s;
}
.header__logo-container:hover {
  color: #7843e9;   
}
.header__logo-img {
    width: 100%;
    height: 100%;
    /* -o-object-fit: cover; */
    object-fit: cover;
    /* -o-object-position: center; */
    object-position: center;
    display: block;
}
.header__logo-sub {
    font-size: 1.6rem;
    text-transform: uppercase;
    font-weight: 700;
    letter-spacing: 1px;
}
</style>