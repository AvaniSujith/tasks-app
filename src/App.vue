<script lang="ts" setup>
import { ref } from "vue";

const message = ref('hello world')
</script>

<template>
  <main>
    <h2>{{ message }}</h2>
  </main>
</template>

<style scoped>
main{
  max-width:  800px;
  margin: 1rem auto;
}
</style>