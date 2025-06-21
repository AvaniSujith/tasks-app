<script lang="ts" setup>
import { ref } from "vue";

const message = ref('hello world');
const newTask = ref("");

function formSubmitted(){
  console.log(newTask.value);
}

</script>

<template>
  <main>
    <h1>{{ message }}</h1>
    <form @submit.prevent="formSubmitted">
      <label>
        New Task
         <input name="newTask" v-model="newTask" >
      </label>
      <div class="button-container">
        <button>Add</button>
      </div>
    </form>
  </main>
</template>

<style scoped>
main{
  max-width:  800px;
  margin: 1rem auto;
}

.button-container{
  display: flex;
  justify-content: end;
}
</style>