<script setup lang="ts">
import PhaserContainer from "@/components/PhaserContainer.vue"
</script>

<template>
  <Suspense>
    <PhaserContainer />

    <template #fallback>
      <div class="font-mono text-2xl">Downloading...</div>
    </template>
  </Suspense>
</template>

<style scoped></style>
