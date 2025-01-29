<template>
  <h1>Equipe</h1>
  <div v-for="c in cargos" :key="c.id">{{ c.cargo }} {{ c.nome }}
    <button @click="store.removeCargo(c.id)">Remover</button>
  </div>
</template>

<script setup>
import { useCargos } from '@/store/cargos';
import { storeToRefs } from 'pinia';

const store = useCargos();

const { cargos } = storeToRefs(store);


</script>

<style scoped></style>