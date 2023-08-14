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

<style scoped>
.heading-sec__main {
  display: block;
  font-size: 3.5rem;
  text-transform: uppercase;
  letter-spacing: 1px;
  letter-spacing: 3px;
  text-align: center;
  margin-bottom: 3.5rem;
  position: relative;
  color: #111;
}
.heading-sec__sub {
  display: block;
  text-align: center;
  color: #555;
  font-size: 2rem;
  font-weight: 500;
  max-width: 80rem;
  margin: auto;
  line-height: 1.6;
}
</style>