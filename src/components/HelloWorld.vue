<script setup lang="ts">
  import { ref } from 'vue'

  defineProps<{ msg: string }>()

  const count = ref(0)
</script>

<template>
  <h1 class="text-2xl py-3 dark:text-white">{{ msg }}</h1>

  <div class="card">
    <button
      class="px-6 py-2 rounded-full bg-emerald-100 hover:bg-emerald-200 text-emerald-500"
      type="button"
      @click="count++"
    >
      count is {{ count }}
    </button>
    <p class="py-2 dark:text-white">
      Edit
      <code class="text-red-400">components/HelloWorld.vue</code> to test HMR
    </p>
  </div>

  <p class="py-2 dark:text-white">
    Check out
    <a
      class="underline text-emerald-500"
      href="https://vuejs.org/guide/quick-start.html#local"
      target="_blank"
      >create-vue</a
    >, the official Vue + Vite starter
  </p>
  <p class="py-2 dark:text-white">
    Install
    <a
      class="underline text-emerald-500"
      href="https://github.com/johnsoncodehk/volar"
      target="_blank"
      >Volar</a
    >
    in your IDE for a better DX
  </p>
  <p class="py-2 dark:text-white">
    Click on the Vite and Vue logos to learn more
  </p>
</template>
