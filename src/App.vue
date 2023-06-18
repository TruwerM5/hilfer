<script setup>
import HelloWorld from './components/HelloWorld.vue'
import HeaderVue from './components/HeaderVue.vue';
import Index from './views/index.vue';
</script>

<template>
  <!-- <HelloWorld /> -->
  <HeaderVue />
  <router-view></router-view>
  <!-- <img src="/images/logo.png" alt="Logo"> -->
</template>


