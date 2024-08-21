<script setup lang="ts">
const breadcrumbs = [
  { name: 'Home', url: '/' },
  { name: 'Sale', url: '/sale' },
  { name: 'Shoes', url: '/sale/shoes' }
]
</script>

<template>
  <ul>
    <li v-for="item in breadcrumbs" v-bind:key="item.url" class="breadcrumb">
      <a :href="item.url">{{ item.name }}</a>
    </li>
  </ul>
</template>

<style scoped>
ul {
  padding: 8px 0 16px 0;
}

.breadcrumb {
  display: inline;
  font-size: 0.875rem;
  color: var(--color-gray-700);

  &:not(:first-of-type)::before {
    content: '/';
    color: var(--color-gray-300);
    margin-inline: 8px;
  }

  & a {
    color: inherit;
    text-decoration: none;

    &:hover {
      text-decoration: underline;
    }
  }
}
</style>
