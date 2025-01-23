<template>
  <nav>
    <span>Projeto vue</span>
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Sobre</a></li>
      <li><a href="#">Login</a></li>
    </ul>
  </nav>
</template>

<script setup>

</script>

<style scoped>
nav {
  padding: 5px;
  display: flex;
  justify-content: space-between;
  align-content: center;
  background: #cae7e8;
}
ul {
  display: flex;
  list-style-type: none;
}
ul li {
  padding: 0 5px;
}
ul li a {
  text-decoration: none;
  color: #117177
}
</style>