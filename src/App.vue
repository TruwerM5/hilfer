<script setup>
import HeaderVue from './components/HeaderVue.vue';
import Index from './views/index.vue';
</script>

<template>
  <!-- <HelloWorld /> -->
  <HeaderVue />
  <main class="main">
    <router-view></router-view>

  </main>
  <!-- <img src="/images/logo.png" alt="Logo"> -->
</template>

<style lang="sass" scoped>
.main
  padding-inline: 300px
</style>


