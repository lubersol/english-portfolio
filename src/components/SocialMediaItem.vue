<script setup>
defineProps({
  icons: {
    type: Array,
  },  
  name: {
    type: String,
    required: false
  },
  text: {
    type: String,
    required: false
  }
})
</script>

<template>
  <div class="home-hero__socials">
    <div v-for="icon in icons" :key="icon.id" class="home-hero__social">
      <a :href="icon.link" class="home-hero__social-icon-link" rel="noreferrer" target="_blank">
        <i :class="icon.name" style="font-size:x-large; color:black; width:100%" :alt="icon.text"></i>
      </a>
    </div>
  </div>
</template>

<style scoped>
.home-hero__socials {
  position: absolute;
  top: 35%;
  transform: translateY(-50%);
  background: #fff;
  box-shadow: rgba(100,100,111,.2) 0 7px 29px 0;
  padding: .5rem;
}
.home-hero__social {
  width: 5rem;
}
.home-hero__social-icon-link {
    width: 100%;
    display: block;
    padding: 1rem;
    /* transition: background .3s; */
    border-radius: 5px;
}
.home-hero__social-icon-link:hover {
    background: rgba(120,67,233,.2);
}

@media only screen and (max-width: 56.25em) {
  .home-hero__socials {
    display: none;
  }
}
</style>
