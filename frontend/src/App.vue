<template>
  <NavBar v-once />
  <header>
    <Header />
  </header>

  <main>
    <!-- <Usuario /> -->
    <router-view></router-view>
  </main>
</template>

<script setup>
import Header from './components/Header.vue';
</script>

<style></style>