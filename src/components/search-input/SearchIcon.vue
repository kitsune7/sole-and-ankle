<script setup lang="ts">
import { defineProps } from 'vue'

interface Props {
  size?: number
}

withDefaults(defineProps<Props>(), {
  size: 24
})
</script>

<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    :width="size"
    :height="size"
    viewBox="0 0 24 24"
    fill="none"
    stroke="currentColor"
    stroke-width="1"
    stroke-linecap="round"
    stroke-linejoin="round"
  >
    <circle cx="11" cy="11" r="8"></circle>
    <line x1="21" y1="21" x2="16.65" y2="16.65"></line>
  </svg>
</template>

<style scoped>
svg {
  display: block;
}
</style>
