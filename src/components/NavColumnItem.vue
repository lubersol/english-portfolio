<script setup>
import { RouterLink } from 'vue-router'

</script>

<template>
  <div class="header__sm-menu">
    <div class="header__sm-menu-content">
      <ul class="header__sm-menu-links">
        <li class="header__sm-menu-link">
          <RouterLink to="/">Home</RouterLink>
        </li>
        <li class="header__sm-menu-link">
          <RouterLink to="/about">About</RouterLink>
        </li>
        <li class="header__sm-menu-link">
          <RouterLink to="/projects">Projects</RouterLink>
        </li>
        <li class="header__sm-menu-link">
          <RouterLink to="/contact">Contact</RouterLink>
        </li>
      </ul>
    </div>
  </div>
</template>

<style>
.header__sm-menu{
  background:#fff;
  position:absolute;
  width:100%;
  top:100%;
  visibility:hidden; 
  opacity:0; 
  transition:all .3s;
  box-shadow:0 5px 5px 0 rgba(0,0,0,.1);
  -webkit-box-shadow:0 5px 5px 0 rgba(0,0,0,.1);
  -moz-box-shadow:0 5px 5px 0 rgba(0,0,0,.1);
}
.header__sm-menu--active{
  visibility:hidden; 
  opacity:0;
}
.header__sm-menu-link a{
  display:block;
  text-decoration:none;
  padding:2.5rem 3rem;
  font-size:1.6rem;
  color:#333;
  text-align:right;
  border-bottom:1px solid #eee;
  font-weight:700;
  text-transform:uppercase;
  letter-spacing:2px;
  transition:color .3s;
}
.header__sm-menu-link a:hover{
  color:#7843e9;
}
.header__sm-menu-link:first-child a{
  border-top:1px solid #eee;
}
.header__sm-menu-link-last{
  border-bottom:0;
} 

</style>
