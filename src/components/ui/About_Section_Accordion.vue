<script lang="ts" setup>
import { ref } from 'vue'

const isFeatureHovered = ref(false)
</script>

<template>
  <div
    class="group/feature"
    @mouseover="isFeatureHovered = true"
    @mouseleave="isFeatureHovered = false"
  >
    <h3 class="group-hover/feature:text-violet-500">Fully Customize the structure of every page</h3>
    <Transition>
      <div v-if="isFeatureHovered">
        <p>
          Drag in unstyled HTML elements to build exactly what you want — then turn footers, nav
          bars, and more into components you can reuse.
        </p>
      </div>
    </Transition>
  </div>
</template>

<style>
.v-enter-active,
.v-leave-active {
  transition:
    transform 0.5s ease,
    opacity 0.5s ease;
}

.v-enter-from,
.v-leave-to {
  transform: translateY(100%);
  opacity: 0;
}
.v-enter-to,
.v-leave-from {
  transform: translateY(0);
  opacity: 1;
}
</style>
