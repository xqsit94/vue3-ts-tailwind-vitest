<script setup lang="ts">
  import HelloWorld from '~/components/HelloWorld.vue'

  const msg =
    'Vue 3 + Vite starter template with TypeScript, Tailwind CSS 3, Vitest and Husky'
</script>

<template>
  <div class="flex flex-col h-screen items-center justify-center">
    <div class="flex justify-center my-4">
      <a href="https://vitejs.dev" target="_blank">
        <img src="/vite.svg" class="logo" alt="Vite logo" />
      </a>
      <a href="https://vuejs.org/" target="_blank">
        <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
      </a>
    </div>
    <div class="text-center">
      <HelloWorld :msg="msg" />
    </div>
  </div>
</template>

<style scoped>
  .logo {
    height: 8em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.vue:hover {
    filter: drop-shadow(0 0 2em #42b883aa);
  }
</style>
