<script setup lang="ts">
import { ref } from 'vue'
import { invoke } from '@tauri-apps/api/core'

const greetMsg = ref('')
const name = ref('')

async function greet() {
  // Learn more about Tauri commands at https://tauri.app/v1/guides/features/command
  greetMsg.value = await invoke('greet', { name: name.value })
}
</script>

<template>
  <form class="w-full flex justify-between gap-5 my-5" @submit.prevent="greet">
    <input id="greet-input" class="border-0 outline-0 p-2 rounded-md bg-neutral-700 focus:bg-neutral-600 w-full" v-model="name" placeholder="Enter a name..." />
    <button type="submit" class="rounded-md bg-purple-400 px-5 hover:cursor-pointer hover:bg-purple-500">Greet</button>
  </form>

  <p class="text-2xl">{{ greetMsg }}</p>
</template>
