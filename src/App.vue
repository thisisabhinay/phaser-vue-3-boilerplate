<script setup lang="ts">
import { RouterLink, RouterView } from "vue-router"
</script>

<template>
  <section class="grid grid-cols-1 gap-10 auto-rows-max max-w-5xl m-auto py-10">
    <header>
      <nav class="flex items-center gap-10 text-blue-500">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </header>
    <h1 class="text-2xl">Phaser.js Boilerplate</h1>
    <RouterView />
  </section>
</template>

<style scoped></style>
