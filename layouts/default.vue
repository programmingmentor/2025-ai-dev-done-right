<script setup lang="ts">
// Default layout with custom background
import { resolveAssetUrl } from "./layoutHelper";
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
</template>

<style>
/* Additional styles if needed */
</style>
