<script setup lang="ts">
import Cart from './Cart.vue'
import SearchInput from './search-input/SearchInput.vue'
</script>

<template>
  <header>
    <div class="super-header">
      <span class="marketing-message">Free shipping on domestic orders over $75!</span>
      <div class="right-section">
        <SearchInput />
        <a href="/help">Help</a>
        <a href="/cart"><Cart /></a>
      </div>
    </div>
    <div class="main-header">
      <a href="/" class="logo"><h1>Sole&Ankle</h1></a>
      <nav>
        <a href="/sale">Sale</a>
        <a href="/new">New&nbsp;Releases</a>
        <a href="/men">Men</a>
        <a href="/women">Women</a>
        <a href="/kids">Kids</a>
        <a href="/collections">Collections</a>
      </nav>
      <span></span>
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

.marketing-message {
  color: var(--color-white);
}

.right-section {
  display: flex;
  align-items: center;
  gap: 16px;
}

.super-header a {
  color: var(--color-gray-300);
  text-decoration: none;

  &:hover {
    color: var(--color-white);
    text-decoration: underline;
  }
}

.main-header {
  align-items: center;
  border-bottom: 1px solid var(--color-gray-300);
  display: flex;
  padding: 0 32px;
  justify-content: space-between;
}

.logo,
.main-header > span {
  flex-grow: 1;
  flex-basis: 0;
}

.logo {
  text-decoration: none;
  color: inherit;

  &:hover {
    color: var(--color-primary);
  }
}
.logo h1 {
  font-size: 1.5rem;
  font-weight: var(--weight-bold);
}

nav {
  display: flex;
  gap: 32px;
  flex-shrink: 0;
}

nav a {
  color: var(--color-gray-900);
  font-size: 1.125rem;
  font-weight: var(--weight-medium);
  text-decoration: none;
  text-transform: uppercase;

  &:first-of-type {
    color: var(--color-secondary);
  }

  &:hover {
    text-decoration: underline;
  }
}
</style>
