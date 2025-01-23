<template>
  <div class="pessoas">
    <Usuario first_name="Cassiano"></Usuario>
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue';
import Usuario from './Usuario.vue';
const pessoas = ref([])

const buscarInformacoes = async () => {
  const req = await fetch(`https://reqres.in/api/users?page=2`)
  const json = await req.json()
  return json.data
};

onMounted(async () => {
  pessoas.value = await buscarInformacoes()
});
</script>

<style scoped>
.pessoas {
  display: flex;
  flex-wrap: wrap;
}

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