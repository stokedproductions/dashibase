<template>
  <div class="flex items-center justify-center rounded-full w-8 h-8 cursor-pointer text-neutral-700 hover:bg-highlight dark:text-neutral-400 dark:hover:bg-highlight-dark"
    @click="store.darkMode = !store.darkMode" title="Toggle dark mode">
    <SunIcon class="w-5 dark:hidden" />
    <MoonIcon class="w-5 hidden dark:block" />
  </div>
</template>

<script setup lang="ts">
import {
  SunIcon,
  MoonIcon,
} from '@heroicons/vue/outline'
import { useStore } from '@/utils/store'

const store = useStore()
</script>
