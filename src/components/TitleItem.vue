<script setup>
defineProps({
  title: {
    type: String,
    required: true
  },
  text: {
    type: String,
    required: false
  },
  subtitle: {
    type: Boolean,
    default: false
  }
})
</script>

<template>
  <h2 class="heading heading-sec heading-sec__mb-med">
    <span class="heading-sec__main">{{ title }}</span>
    <span v-if="subtitle" class="heading-sec__sub">
      {{ text }}
    </span>
  </h2>
</template>

