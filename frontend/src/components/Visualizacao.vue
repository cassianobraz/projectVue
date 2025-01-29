<template>
  <NavBar v-once />
  <header>
    <Header />
  </header>

  <main>
    <slot></slot>
  </main>
</template>

<script setup>
import Header from './Header.vue';
</script>

<style></style>