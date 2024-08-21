<script setup lang="ts">
import { Head } from '@unhead/vue/components'
import Header from './components/Header.vue'
import Sidebar from './components/Sidebar.vue'
import ShoeView from './components/ShoeView.vue'
</script>

<template>
  <Head>
    <meta charset="utf-8" />
    <link rel="icon" href="/favicon.ico" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="theme-color" content="#000000" />
    <meta name="description" content="Web site created using Vue3" />

    <link rel="preconnect" href="https://fonts.gstatic.com" />
    <link
      href="https://fonts.googleapis.com/css2?family=Raleway:wght@500;600;800&display=swap"
      rel="stylesheet"
    />

    <title>Sole&Ankle — CSS for JavaScript Developers</title>
  </Head>

  <Header />
  <main>
    <Sidebar />
    <ShoeView />
  </main>
</template>

<style scoped>
main {
  align-items: flex-start;
  display: flex;
  gap: 64px;
  padding: 64px 32px;
}
</style>
