<script lang="ts" setup>
import { ref } from "vue";

const message = ref('hello world');
const newTask = ref("");
</script>

<template>
  <main>
    <h2>{{ message }}</h2>
    <input name="newTask" v-model="newTask" >
    <p>{{ newTask }}</p>
  </main>
</template>

<style scoped>
main{
  max-width:  800px;
  margin: 1rem auto;
}
</style>