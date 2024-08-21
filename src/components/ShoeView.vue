<template>
  <section>
    <h2>Running</h2>
    <div class="filter">
      <button>Sort</button>
      <select>
        <option>Newest Releases</option>
        <option>Best Sellers</option>
      </select>
    </div>
  </section>
</template>

<style scoped>
section {
  align-items: center;
  display: flex;
  justify-content: space-between;
  flex-grow: 1;
}

button {
  background-color: transparent;
  border: 0;
  color: var(--color-gray-700);
  cursor: pointer;

  &:hover {
    color: var(--color-gray-900);
  }
}

select {
  cursor: pointer;
}

.filter {
  display: flex;
  gap: 8px;
}
</style>
