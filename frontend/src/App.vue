<template>
  <NavBar />
  <header>
    <Header />
  </header>

  <main>
    <Usuario />
  </main>
</template>

<script setup>
import Header from './components/Header.vue';
import Usuario from './components/Usuario.vue';
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}
header {
  line-height: 1.5;
}
</style>