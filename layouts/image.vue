<script setup lang="ts">
import { computed } from "vue";
import { handleBackground, resolveAssetUrl } from "./layoutHelper";
import TelegramLogo from "../components/TelegramLogo.vue";

const props = defineProps({
  image: {
    type: String,
  },
  class: {
    type: String,
  },
  backgroundSize: {
    type: String,
    default: "cover",
  },
});

const style = computed(() =>
  handleBackground(props.image, false, props.backgroundSize),
);
</script>

<template>
  <div
    class="slidev-layout"
    :class="props.class"
    :style="style"
    style="position: relative; overflow: hidden"
  >
    <!-- Apply global background -->
    <div
      :style="{
        position: 'absolute',
        top: 0,
        left: 0,
        width: '100%',
        height: '100%',
        backgroundImage: `url('${resolveAssetUrl('/dou-bg-dark-01.png')}')`,
        backgroundSize: 'cover',
        backgroundPosition: 'center',
        backgroundRepeat: 'no-repeat',
        zIndex: -2,
      }"
    ></div>
    <!-- Content -->
    <slot />
  </div>
  <TelegramLogo />
</template>
