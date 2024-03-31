<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Greet from './components/Greet.vue'
</script>

<template>
  <div class="w-dvh h-dvh dark:bg-neutral-800 dark:text-white p-10">
    <h1 class="text-6xl text-center">Welcome to Tauri!</h1>

    <div class="w-full flex justify-evenly my-10">
      <a href="https://vitejs.dev" target="_blank">
        <img src="/vite.svg" class="w-12" alt="Vite logo" />
      </a>
      <a href="https://tauri.app" target="_blank">
        <img src="/tauri.svg" class="w-12" alt="Tauri logo" />
      </a>
      <a href="https://vuejs.org/" target="_blank">
        <img src="./assets/vue.svg" class="w-12" alt="Vue logo" />
      </a>
    </div>

    <p class="text-sm text-center my-1">
      Click on the
      <span class="text-purple-400 hover:text-purple-500 hover:cursor-pointer"
        >Tauri</span
      >,
      <span class="text-purple-400 hover:text-purple-500 hover:cursor-pointer"
        >Vite</span
      >, and
      <span class="text-purple-400 hover:text-purple-500 hover:cursor-pointer"
        >Vue</span
      >
      logos to learn more.
    </p>

    <Greet />

    <div class="absolute bottom-2 right-2 text-sm dark:text-white">
      <p>
        Recommended IDE setup:
        <a href="https://code.visualstudio.com/" class="text-purple-400" target="_blank">VS Code</a>
        +
        <a href="https://github.com/johnsoncodehk/volar" class="text-purple-400" target="_blank">Volar</a>
        +
        <a href="https://github.com/tauri-apps/tauri-vscode" class="text-purple-400" target="_blank"
          >Tauri</a
        >
        +
        <a href="https://github.com/rust-lang/rust-analyzer" target="_blank"
          >rust-analyzer</a
        >
      </p>
    </div>
  </div>
</template>
