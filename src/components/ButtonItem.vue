<script setup>
import { RouterLink } from 'vue-router'

defineProps({
  text: {
    type: String,
    required: true
  },
  href: {
    type: String,
    required: true
  },
})
</script>

<template>
  <div class="home-hero__cta">
    <RouterLink :to="href" class="btn btn--bg">{{ text }}</RouterLink>
  </div>
</template>


