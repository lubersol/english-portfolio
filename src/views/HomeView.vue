<script setup>
import ButtonItem from '@/components/ButtonItem.vue'
import SocialMediaItem from '@/components/SocialMediaItem.vue'
import { BASE_URL } from 'vue-router'

</script>

<template>
  <div class="home-hero">
    <div class="home-hero__content">
      <h1 class="heading-primary">Hey, I'm Lucía Bermejo</h1>
      <div class="home-hero__info">
        <p class="text-primary">
          A Fullstack focused Web Developer building the Frontend of Websites
          and Web Applications that leads to the success of the overall
          product
        </p>
      </div>
      <ButtonItem text="Projects" :href="`${BASE_URL}projects`" />
    </div>  
  </div>
  <SocialMediaItem />
</template>

