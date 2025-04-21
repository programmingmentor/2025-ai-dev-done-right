<script setup lang="ts">
// Default layout with custom background
</script>

<template>
  <div
    class="slidev-layout default"
    style="
      background-image: url(&quot;/dou-bg-dark-01.png&quot;);
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
    "
  >
    <slot />
  </div>
</template>

<style>
/* Additional styles if needed */
</style>
