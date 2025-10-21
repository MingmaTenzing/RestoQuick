<script setup lang="ts">
import { useDark, useToggle } from '@vueuse/core'
const isDark = useDark()
const toggleDark = useToggle(isDark)
</script>

<template>
  <p class="">hello world peace</p>
  <p class="">the theme mode is {{ isDark }}</p>
  <button v-on:click="toggleDark()" class="border px-4 p-2 rounded-lg bg-accent">DarkMode</button>
  <button class="border px-4 p-2 rounded-lg bg-accent">LightMode</button>
</template>
