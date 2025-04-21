<template>
  <div class="ssa-logo-global" v-if="$slidev.nav.currentLayout !== 'end'">
    <a href="https://career.softserveinc.com/uk-ua/softserve-academy">
      <img src="/ssa-logo-white.svg" alt="SoftServe Academy Logo" />
    </a>
  </div>
  <div class="dou-logo-global" v-if="$slidev.nav.currentPage !== 1">
    <a href="https://dou.ua/">
      <img src="/dou-day-logo-color.png" alt="DOU Logo" />
    </a>
  </div>
  <div class="city-year-text" v-if="$slidev.nav.currentPage !== 1">
    Київ, 2025
  </div>
</template>

<style>
.ssa-logo-global {
  position: fixed;
  bottom: 10px;
  right: 20px;
  z-index: 100;
  pointer-events: auto;
}

.ssa-logo-global img {
  height: 13px;
  width: auto;
}

.ssa-logo-global a {
  text-decoration: none;
  border: 2.4px solid transparent;
  display: block;
}

.ssa-logo-global a:hover {
  border-color: var(--slidev-theme-primary);
}

.dou-logo-global {
  position: fixed;
  top: 10px;
  right: 20px;
  z-index: 100;
  pointer-events: auto;
}

.dou-logo-global img {
  height: 20px;
  width: auto;
}

.dou-logo-global a {
  text-decoration: none;
  border: 2.4px solid transparent;
  display: block;
}

.dou-logo-global a:hover {
  border-color: var(--slidev-theme-primary);
}

.city-year-text {
  position: fixed;
  top: 10px;
  left: 20px;
  z-index: 100;
  color: white;
  font-size: 14px;
  font-weight: 500;
}
</style>
