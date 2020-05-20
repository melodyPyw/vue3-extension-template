<template>
  <div id="app">
    {{count}}
    <button @click="handleAdd">add</button>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    const count = ref(0)
    const handleAdd = () => {
      count.value++
    }
    return {
      count,
      handleAdd
    }
  },
}
</script>

<style>
</style>
