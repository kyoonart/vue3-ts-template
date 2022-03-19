<script setup lang="ts">
import { useMainStore } from '@/store/main'
import { ref } from 'vue'
import { NButton } from 'naive-ui'

const mainStore = useMainStore()

// defineProps<{ msg: string }>()

const count = ref(0)
</script>

<template>
  <div>
    <h1>welcome to vue3</h1>
    <div>{{ mainStore.name }}</div>
    <n-button>naive-ui</n-button>
  </div>
</template>

<style scoped>
a {
  color: #42b983;
}

label {
  margin: 0 0.5em;
  font-weight: bold;
}

code {
  background-color: #eee;
  padding: 2px 4px;
  border-radius: 4px;
  color: #304455;
}
</style>
