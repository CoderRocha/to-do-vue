<script setup>

import {ref} from 'vue'

const emit = defineEmits(['addTask'])
const newTask = ref('')
const addTask = () => {
  if (!newTask.value) return
  
  emit('addTask', newTask.value)
  newTask.value = ''
}

</script>

<template>
    <div class="input-group mb-3">
      <!-- {{ newTask }} -->
      <input v-model="newTask" @keyup.enter="addTask" type="text" placeholder="Adicionar uma nova tarefa..." class="form-control">
      <button @click="addTask" class="btn btn-success">Adicionar</button>
    </div>
</template>