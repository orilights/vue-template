<script setup lang="ts">
import { useStore } from '@/store'

const store = useStore()
const { count } = toRefs(store)
</script>

<template>
  <div class="flex h-screen flex-col items-center justify-center">
    <HelloWorld />
    <button class="rounded-md border px-2 py-1 hover:border-blue-500" @click="count++">
      Count: {{ count }}
    </button>
  </div>
</template>
