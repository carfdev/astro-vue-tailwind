<script setup lang="ts">
import { ref } from 'vue';

const count = ref<number>(0);
</script>

<template>
  <div>
    <p>Count: {{ count }}</p>
    <button @click="count++">Increment</button>
  </div>
</template>

<style scoped>
@reference '@/styles/global.css';

div {
  @apply mt-10 flex flex-col items-center gap-4;
}

p {
  @apply text-2xl;
}

button {
  @apply cursor-pointer rounded bg-blue-500 px-4 py-2 text-white;
}
</style>
