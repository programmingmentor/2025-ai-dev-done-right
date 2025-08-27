<template>
  <div class="telegram-logo-container">
    <a
      :href="telegramUrl"
      target="_blank"
      rel="noopener noreferrer"
      class="logo-link"
      :title="tooltipText"
    >
      <img src="/pm-logo.jpg" alt="PM Logo" class="pm-logo" />
    </a>
    <a
      :href="telegramUrl"
      target="_blank"
      rel="noopener noreferrer"
      class="channel-name-link"
      :title="tooltipText"
    >
      <div class="channel-name">{{ channelName }}</div>
    </a>
  </div>
</template>

<script setup>
// Component for displaying PM logo with Telegram link
import { telegramConfig } from "./TelegramConfig.js";

const telegramUrl = telegramConfig.channelUrl;
const tooltipText = telegramConfig.tooltipText;
const channelName = telegramConfig.channelName;

// Get logo size from config
const logoSize = telegramConfig.logo.size.desktop;
const mobileLogoSize = telegramConfig.logo.size.mobile;
</script>

<style scoped>
.telegram-logo-container {
  position: fixed;
  bottom: 20px;
  right: 20px;
  z-index: 1000;
}

.logo-link {
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: all 0.3s ease;
  color: white;
  text-decoration: none !important;
  text-decoration-line: none !important;
  border-bottom: 0 !important;
  display: inline-block;
}

.logo-link:hover,
.logo-link:focus,
.logo-link:active,
.logo-link:visited {
  transform: scale(1.05);
  text-decoration: none !important;
  text-decoration-line: none !important;
  border-bottom: 0 !important;
}

.channel-name {
  font-size: 10px;
  font-weight: 500;
  margin-top: 4px;
  text-align: center;
  color: rgba(255, 255, 255, 0.8);
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.5);
  white-space: nowrap;
  text-decoration: none !important;
}

.pm-logo {
  width: v-bind(logoSize);
  height: v-bind(logoSize);
  border-radius: 50%;
  border: 3px solid rgba(255, 255, 255, 0.4);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
  object-fit: cover;
}

/* Responsive design */
@media (max-width: 768px) {
  .pm-logo {
    width: v-bind(mobileLogoSize);
    height: v-bind(mobileLogoSize);
  }

  .telegram-logo-container {
    bottom: 15px;
    right: 15px;
  }

  .channel-name {
    font-size: 8px;
    margin-top: 2px;
  }
}

/* Ensure channel name never has text decoration */
.channel-name-link,
.channel-name-link:hover,
.channel-name-link:visited,
.channel-name-link:active,
.telegram-logo-container .channel-name,
.telegram-logo-container .channel-name:hover,
.telegram-logo-container .channel-name:visited,
.telegram-logo-container .channel-name:active {
  text-decoration: none !important;
}

/* Specific styles for image-left layout */
.slidev-layout[class*="image-left"] .telegram-logo-container .channel-name {
  text-decoration: none !important;
}

/* Global override for all layouts */
.slidev-layout .telegram-logo-container .channel-name {
  text-decoration: none !important;
}
</style>
