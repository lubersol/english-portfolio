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

<style scoped>
.btn:hover {
    transform: translateY(-3px);
}
.btn--bg {
  padding: 1.5rem 8rem;
  font-size: 2rem;
}
.btn {
  background: #7843e9;
  color: #fff;
  text-transform: uppercase;
  letter-spacing: 1px;
  display: inline-block;
  font-weight: 700;
  border-radius: 5px;
  box-shadow: 0 5px 15px 0 rgba(0,0,0,.15);
  transition: transform .3s;
}

a {
  text-decoration: none;
  color: inherit;
}

*, ::after, ::before {
    margin: 0;
    padding: 0;
    box-sizing: inherit;
    font-family: inherit;
}
.home-hero__cta {
    margin-top: 5rem;
    text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
