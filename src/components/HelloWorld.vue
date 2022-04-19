<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
</script>

<template>
  <h1 class="mb-5 text-3xl font-bold underline">{{ msg }}</h1>


  <p>
    <a href="https://www.electronjs.org/docs/latest/" target="_blank">
      Electron Documentation
    </a>
    |
    <a href="https://tailwindcss.com/docs/installation" target="_blank">
      tailwindcss Documentation
    </a>
  </p>

  <p>
    <a href="https://vitejs.dev/guide/features.html" target="_blank">
      Vite Documentation
    </a>
    |
    <a href="https://v3.vuejs.org/" target="_blank">Vue 3 Documentation</a>
  </p>

  <button type="button" @click="count++">count is: {{ count }}</button>
  <p>
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<style scoped>
a {
  color: #4272b9;
}
</style>
