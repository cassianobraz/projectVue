<template>
  <div>
    <form class="formulario">
      <label for="nome">Nome:</label><br>
      <input type="text" id="nome" name="nome" v-model="nome"><br>
      <label for="dataNascimento">Data Nascimento:</label><br>
      <input type="number" id="dataNascimento" name="dataNascimento" v-model="dataNascimento"><br>
    </form>
  </div>
  <p style="text-align: center">{{ nome }} nasceu em {{ dataNascimento }}</p>
</template>

<script setup>
import { ref } from "vue";
const nome = ref('Cassiano')
const dataNascimento = ref(0)
const idade = ref(10)
console.log(idade.value);

</script>

<style scoped>
.formulario {
  margin: 0 auto;
  padding: 5px;
  width: 200px;
  background: darkcyan;
}
</style>