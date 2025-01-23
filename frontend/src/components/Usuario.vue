<template>
  <div class="perfil">
    <img :src="pessoa.avatar" alt="Perfil">
    <strong>{{ first_name }}</strong>
  </div>
</template>

<script setup>
import { computed } from 'vue';

// const nomeCompleto = computed(() => `${pessoa.value.first_name} ${pessoa.value.last_name}`)
defineProps({
  first_name: String,
})
</script>

<style scoped>
.perfil {
  width: 150px;
  text-align: center;
}

.perfil img {
  margin: 0 auto;
  width: 80px;
  display: block;
  padding: 5px;
  border-radius: 10px;
}

.perfil span {
  display: block;
  font-size: 0.75rem;
}
</style>