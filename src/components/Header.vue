<template>
  <header>
    <div class="super-header">
      <span class="marketing-message">Free shipping on domestic orders over $75!</span>
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
  font-size: 0.875rem;
  color: var(--color-gray-300);
  background-color: var(--color-gray-900);
  padding: 10px;
  text-align: center;
}
.marketing-message {
  color: white;
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
