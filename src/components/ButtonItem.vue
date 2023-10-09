<script setup>
import { defineProps, computed } from 'vue'

const { text, href } = defineProps(['text', 'href'])

const absoluteHref = computed(() => {
  // Utiliza import.meta.env.BASE_URL para obtener la ruta base
  const BASE_URL = import.meta.env.BASE_URL
  return `${BASE_URL}${href}`
})

// defineProps({
//   text: {
//     type: String,
//     required: true
//   },
//   // href: {
//   //   type: String,
//   //   required: true
//   // },
// })
</script>

<template>
  <div class="home-hero__cta">
    <a :href="absoluteHref" class="btn btn--bg">{{ text }}</a>
  </div>
</template>


