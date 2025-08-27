# Налаштування Telegram-каналу

## Що було додано

На всі слайди презентації додано лого з лінком на ваш Telegram-канал. Лого відображається у правому нижньому куті кожного слайду.

## Як налаштувати

1. Відкрийте файл `components/TelegramConfig.js`
2. Замініть `"https://t.me/your_telegram_channel"` на URL вашого Telegram-каналу
3. При бажанні змініть текст підказки (tooltip)

### Приклад налаштування:

```javascript
export const telegramConfig = {
  // Ваш Telegram-канал
  channelUrl: "https://t.me/pm_channel",

  // Текст підказки при наведенні
  tooltipText: "Підписуйтесь на мій Telegram-канал!",

  // Налаштування лого
  logo: {
    size: {
      desktop: "70px",
      mobile: "50px",
    },
    position: {
      bottom: "20px",
      right: "20px",
    },
  },
};
```

## Файли, які були змінені

- `components/TelegramLogo.vue` - компонент лого
- `components/TelegramConfig.js` - конфігурація
- `layouts/default.vue` - додано компонент
- `layouts/center.vue` - додано компонент
- `layouts/image.vue` - додано компонент
- `layouts/image-left.vue` - додано компонент
- `layouts/image-left-bg-color.vue` - додано компонент

## Особливості

- Лого має анімацію при наведенні
- Адаптивний дизайн для мобільних пристроїв
- Використовує ваше лого з файлу `public/pm-logo.jpg`
- Відкривається в новій вкладці

## Як видалити

Якщо потрібно видалити лого з усіх слайдів, просто видаліть рядок `<TelegramLogo />` з усіх файлів layouts.
