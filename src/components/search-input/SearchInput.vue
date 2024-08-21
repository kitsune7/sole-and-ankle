<script setup lang="ts">
import SearchIcon from './SearchIcon.vue'
</script>

<template>
  <div class="wrapper">
    <SearchIcon class="icon" :size="18" />
    <input type="search" placeholder="Search..." />
  </div>
</template>

<style scoped>
.wrapper {
  position: relative;
}

.icon {
  color: inherit;
  top: 50%;
  transform: translateY(-50%);
  position: absolute;
}

input[type='search'] {
  --search-icon-size: 18px;
  background-color: transparent;
  border: 0;
  border-bottom: 1px solid var(--color-gray-300);
  color: var(--color-white);
  padding-left: calc(var(--search-icon-size) + 0.25rem);

  &::placeholder {
    color: var(--color-gray-300);
  }

  &:hover,
  &:focus {
    border-color: var(--color-white);
  }
}
</style>
