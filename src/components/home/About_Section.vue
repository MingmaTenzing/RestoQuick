<script setup lang="ts">
import { ref } from 'vue'
import About_Section_Accordion from '../ui/About_Section_Accordion.vue'

interface accordionItems {
  value: string
  title: string
  content: string
}

const defaultValue = 'item-1'

const accordionItems = ref<accordionItems[]>([
  {
    value: 'item-1',
    title: 'Blazing Fast Performance',
    content:
      'Experience instant load times and smooth navigation—RestroMate is optimized for speed and reliability.',
  },
  {
    value: 'item-2',
    title: 'Install on Any Device',
    content:
      'Use RestroMate anywhere—desktop, tablet, or mobile. It works like a native app once installed.',
  },
  {
    value: 'item-3',
    title: 'Offline Support',
    content:
      'Continue managing your restaurant even without internet. All changes sync automatically when you’re back online.',
  },
  {
    value: 'item-4',
    title: 'Free Basic Version',
    content:
      'Access all essential features—roster, stock, and bookings—without any subscription fees.',
  },
  {
    value: 'item-5',
    title: 'All-in-One Dashboard',
    content:
      'Get everything you need in one place—staff schedules, inventory, bookings, and daily tasks.',
  },
  {
    value: 'item-6',
    title: 'Secure Data Handling',
    content:
      'Your information is encrypted and safely stored locally and in the cloud for peace of mind.',
  },
  {
    value: 'item-7',
    title: 'Multi-Restaurant Management',
    content:
      'Manage multiple branches easily with separate tracking and reports for each location.',
  },
  {
    value: 'item-8',
    title: 'Simple & Intuitive Design',
    content:
      'Built for everyone—no tech skills required. RestroMate’s interface is clean, modern, and easy to use.',
  },
])
</script>

<template>
  <div class="py-10">
    <section class="space-y-4 lg:w-1/2">
      <h2 class="text-5xl md:text-6x">Modern and Powerful App that simplifies your work</h2>
      <p>
        Restro Mate helps you easily create roster, manage stocks and all the essential parts of
        restaurant easily.
      </p>
      <button class="bg-violet-500 px-4 py-2 text-white">Start Using</button>
    </section>

    <section><About_Section_Accordion></About_Section_Accordion></section>
  </div>
</template>
