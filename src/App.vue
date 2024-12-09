<script setup>
import { ref } from "vue";

const tarefas = ref(["Entregar o desafio", "Estudar", "Trabalho"]);

const removerTarefa = () => {};
</script>

<template>
  <h1>Lista de Tarefas</h1>
  <ul>
    <li v-for="(tarefa, index) in tarefas" :key="index">
      {{ tarefa }} <button>❎ Remover</button>
    </li>
  </ul>
</template>

<style></style>
