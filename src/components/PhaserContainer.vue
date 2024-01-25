<script setup lang="ts">
import { onMounted, onUnmounted } from "vue"
import type { Game } from "phaser"

let gameInstance: Game | null = null

const CONTAINER_ID = "PhaserContainer"
const game = await import("@/game")

onMounted(() => {
  gameInstance = game.launch(CONTAINER_ID)
})

onUnmounted(() => {
  gameInstance?.destroy(false)
})
</script>

<template>
  <div :id="CONTAINER_ID" />
</template>
