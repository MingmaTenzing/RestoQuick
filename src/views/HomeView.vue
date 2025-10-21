<script setup lang="ts">
import NavBar from '@/components/home/NavBar.vue'
import TitleSection from '@/components/home/TitleSection.vue'
</script>

<template>
  <main
    class="bg-background bg-[linear-gradient(to_right,#8080800a_1px,transparent_1px),linear-gradient(to_bottom,#8080800a_1px,transparent_1px)] bg-[size:14px_24px] dark:bg-[oklch(0.14_0_0)] dark:bg-[linear-gradient(to_right,#ffffff1a_1px,transparent_1px),linear-gradient(to_bottom,#ffffff1a_1px,transparent_1px)]"
  >
    <div class="lg:w-[1200px] m-auto p-4">
      <NavBar />
      <TitleSection></TitleSection>
    </div>
  </main>
</template>
