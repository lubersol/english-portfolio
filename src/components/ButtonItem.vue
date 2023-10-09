<script setup>
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
    <a :href="href" class="btn btn--bg">{{ text }}</a>
  </div>
</template>


