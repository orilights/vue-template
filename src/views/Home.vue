<script setup lang="ts">
import { useStore } from '@/store'

const store = useStore()
const { count } = toRefs(store)
</script>

<template>
  <div class="flex flex-col items-center justify-center h-screen">
    <HelloWorld />
    <button
      class="px-2 py-1 border rounded-md hover:border-blue-500"
      @click="count++"
    >
      Count: {{ count }}
    </button>
  </div>
</template>
