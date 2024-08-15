<script setup lang="ts">
import Cart from './Cart.vue'
</script>

<template>
  <header>
    <div class="super-header">
      <span class="marketing-message">Free shipping on domestic orders over $75!</span>
      <div class="right-section">
        <input type="search" placeholder="Search..." />
        <a href="/help">Help</a>
        <a href="/cart"><Cart /></a>
      </div>
    </div>
    <div class="main-header">
      <nav>
        <a href="/sale">Sale</a>
        <a href="/new">New&nbsp;Releases</a>
        <a href="/men">Men</a>
        <a href="/women">Women</a>
        <a href="/kids">Kids</a>
        <a href="/collections">Collections</a>
      </nav>
    </div>
  </header>
</template>

<style scoped>
.super-header {
  align-items: center;
  background-color: var(--color-gray-900);
  color: var(--color-gray-300);
  display: flex;
  font-size: 0.875rem;
  justify-content: space-between;
  padding: 8px 32px;
}
.super-header a {
  color: var(--color-gray-300);
  text-decoration: none;
}
.super-header a:hover {
  color: var(--color-white);
  text-decoration: underline;
}
.marketing-message {
  color: var(--color-white);
}
.right-section {
  display: flex;
  align-items: center;
  gap: 16px;
}
input[type='search'] {
  background-color: transparent;
  border: 0;
  border-bottom: 1px solid var(--color-gray-300);
  color: var(--color-white);
}
input[type='search']::placeholder {
  color: var(--color-gray-300);
}

.main-header {
  padding: 0 32px;
  border-bottom: 1px solid var(--color-gray-300);
}
nav a {
  font-size: 1.125rem;
  text-transform: uppercase;
  text-decoration: none;
  color: var(--color-gray-900);
  font-weight: var(--weight-medium);

  &:first-of-type {
    color: var(--color-secondary);
  }
}
</style>
