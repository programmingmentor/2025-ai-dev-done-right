<script setup>
import { resolveAssetUrl } from "./layoutHelper";
import TelegramLogo from "../components/TelegramLogo.vue";
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
  <TelegramLogo />
</template>
