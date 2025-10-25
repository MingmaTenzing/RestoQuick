<script setup lang="ts">
import About_Section from '@/components/home/About_Section.vue'
import Features from '@/components/home/Features.vue'
import NavBar from '@/components/home/NavBar.vue'
import TitleSection from '@/components/home/TitleSection.vue'
import BackgroundGrid from '@/components/ui/BackgroundGrid.vue'
</script>

<template>
  <main class="">
    <section class="lg:w-[1200px] m-auto p-4">
      <NavBar />
    </section>
    <section>
      <!-- the hero section  with gradient background-->
      <BackgroundGrid class="">
        <div class="lg:w-[1200px] m-auto p-4">
          <TitleSection></TitleSection>
        </div>
      </BackgroundGrid>
    </section>

    <section class="lg:w-[1200px] m-auto p-4">
      <!-- start of features section aftert the main image -->
      <Features />
    </section>

    <section>
      <div class="lg:w-[1200px] m-auto p-4">
        <About_Section />
      </div>
    </section>
  </main>
</template>
