<script setup>
import { BASE_URL } from 'vue-router'

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
    <a :href="`${BASE_URL}projects`" class="btn btn--bg">{{ text }}</a>
  </div>
</template>


