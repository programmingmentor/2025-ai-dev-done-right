<script setup>
import { resolveAssetUrl } from "./layoutHelper";
</script>

<template>
  <div
    class="slidev-layout center"
    :style="{
      backgroundImage: `url('${resolveAssetUrl('/dou-bg-dark-01.png')}')`,
      backgroundSize: 'cover',
      backgroundPosition: 'center',
      backgroundRepeat: 'no-repeat',
    }"
  >
    <div class="my-auto">
      <slot />
    </div>
  </div>
</template>
