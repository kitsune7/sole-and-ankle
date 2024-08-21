<script setup lang="ts">
import Breadcrumbs from './Breadcrumbs.vue'
</script>

<template>
  <aside>
    <Breadcrumbs />

    <nav>
      <a href="/lifestyle">Lifestyle</a>
      <a href="/jordan">Jordan</a>
      <a class="active" href="/running">Running</a>
      <a href="/basketball">Basketball</a>
      <a href="/training">Training &amp; Gym</a>
      <a href="/football">Football</a>
      <a href="/skateboarding">Skateboarding</a>
      <a href="/us-football">American Football</a>
      <a href="/baseball">Baseball</a>
      <a href="/golf">Golf</a>
      <a href="/tennis">Tennis</a>
      <a href="/athletics">Athletics</a>
      <a href="/walking">Walking</a>
    </nav>
  </aside>
</template>

<style scoped>
a {
  display: block;
  text-decoration: none;
  font-weight: var(--font-weight-medium);
  color: var(--color-gray-900);
  line-height: 2;

  &:hover {
    text-decoration: underline;
  }
}

.active {
  color: var(--color-primary);
}
</style>
