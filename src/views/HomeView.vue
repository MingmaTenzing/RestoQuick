<script setup lang="ts">
import Features from '@/components/home/Features.vue'
import NavBar from '@/components/home/NavBar.vue'
import TitleSection from '@/components/home/TitleSection.vue'
import BackgroundGrid from '@/components/ui/BackgroundGrid.vue'
</script>

<template>
  <main class="gap-6">
    <!-- gradient grid background -->
    <div class="lg:w-[1200px] m-auto p-4">
      <NavBar />
    </div>
    <BackgroundGrid class="">
      <div class="lg:w-[1200px] m-auto p-4">
        <TitleSection></TitleSection>
      </div>
    </BackgroundGrid>

    <section class="lg:w-[1200px] m-auto p-4">
      <!-- start of features section aftert the main image -->
      <Features />
    </section>
  </main>
</template>
