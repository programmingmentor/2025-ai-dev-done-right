<script setup lang="ts">
// Default layout with custom background
import { resolveAssetUrl } from "./layoutHelper";
import TelegramLogo from "../components/TelegramLogo.vue";
</script>

<template>
  <div
    class="slidev-layout default"
    :style="{
      backgroundImage: `url('${resolveAssetUrl('/dou-bg-dark-01.png')}')`,
      backgroundSize: 'cover',
      backgroundPosition: 'center',
      backgroundRepeat: 'no-repeat',
    }"
  >
    <slot />
  </div>
  <TelegramLogo />
</template>

<style>
/* Additional styles if needed */
</style>
