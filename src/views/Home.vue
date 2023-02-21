<template>
  <div class="h-screen flex flex-col items-center justify-center">
    <HelloWorld />
    <button
      class="px-2 py-1 rounded-md border hover:border-blue-500"
      @click="count++"
    >
      Count: {{ count }}
    </button>
  </div>
</template>

<script setup lang="ts">
const count = ref(1)
</script>
