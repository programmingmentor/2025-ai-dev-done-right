---
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: /dou-first-slide-bg.png
# some information about your slides (markdown enabled)
title: Cursor, Windsurf, Copilot, Cline — найкращі практики розробки з ШІ
info: |
  ## Презентація для DOU

# apply unocss classes to the current slide
# class: text-center  <-- Removing default text-center for more control
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# take snapshot for each slide in the overview
overviewSnapshots: true

# Configure fonts (https://sli.dev/custom/config-fonts.html)
fonts:
  sans: "IBM Plex Sans"
  # Optional: specify weights and italic if needed
  # weights: '400,500,700'
  # italic: false
---

<!-- DOU Logo Top Right -->
<div class="absolute top-4 right-5 z-10">
  <img src="/dou-day-logo-bw.png" alt="DOU Logo BW" style="height: 60px;" />
</div>

<div class="absolute top-1/3 left-[20%] text-white text-lg z-10" style="margin-top: -40px; background-color: black; padding: 10px;">
  Київ, 2025
</div>

<!-- Wrapper Div for Both Blocks -->
<div class="absolute top-1/3 left-[20%] w-3/5 z-10">
  <!-- Black Title Div -->
  <div class="p-6" style="background-color: black;">
    <h1 class="text-white font-black uppercase tracking-wide leading-none" style="font-size: 30px; line-height: 1;">
      Cursor, Windsurf, Copilot, Cline — найкращі практики розробки з ШІ
    </h1>
  </div>
  <!-- Pink Subtitle Div (moved back inside, width adjusted) -->
  <div class="p-4 w-2/3 ml-1/2" style="background-color: rgb(255, 22, 177);"> <!-- Adjusted width to w-2/3 -->
    <p class="text-white text-sm">
      В'ячеслав Колдовський, SoftServe
    </p>
  </div>
</div>

---
layout: image-left
image: /prince-of-persia.webp
---

<div class="h-full flex items-center">
  <h1>Чи пам'ятаєте ви той момент, коли захотіли стати розробником?</h1>
</div>

---
layout: image-left-bg-color
image: /troll-face.png
bgColor: white
backgroundSize: contain
---

<div class="h-full flex items-center">
  <h1>А коли ви почали писати код, чи пам'ятаєте свої перші враження?</h1>
</div>

---

# Всім знайомо :)

<div class="w-full flex justify-center items-center space-x-4 mt-10">
  <img src="/meme-dot1-dot2.jpg" width="200px" class="rounded shadow"/>
  <img src="/meme-works-doesnt-work.jpg" width="200px" class="rounded shadow"/>
  <img src="/meme-regex.jpeg" width="200px" class="rounded shadow"/>
  <img src="/meme-error-line-42.jpg" width="200px" class="rounded shadow"/>
</div>

<!--
https://www.reddit.com/r/compsci/comments/1d2pb75/01_02_030000000000000004_in_depth/
-->

---

# Vibe Coding

<div class="w-full flex justify-center">
  <img src="/vibe-coding-tweet.png" class="w-1/2"/>
</div>

---

# Пітер Левелс

<div class="w-full flex justify-center">
  <div class="ml-20"> 
    <img src="/levelsio.png" class="w-100 h-auto"/>
  </div>
  <div class="ml-20"> 
    <Tweet scale="0.55" id="1901660771505021314" class="w-100"/>
  </div>
</div>

---

<div class="w-full flex justify-center">
  <img src="/personal-motivation-calendar.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center items-center space-x-8 mt-10">
  <a href="https://personalmotivationcalendar.com/">https://personalmotivationcalendar.com/</a>
  <img src="/qr-personalmotivationcalendar.png" class="w-1/8"/>
</div>

---

# Завдання, для яких генерація коду за допомогою ШІ вже працює сьогодні

- MVP
- Хобі-проекти
- "Одноразові" завдання
- Експерименти та прототипи
- ...

---

# Але...

<div class="w-full flex justify-center">
  <img src="/meme-not-so-simple.jpg" class="rounded shadow"/>
</div>

---

# Невдачі - SaaS

<div class="w-full flex justify-center">
  <img src="/fail-saas.png" class="w-1/3"/>
</div>

---

# Невдачі - Fetch

<div class="w-full flex justify-center">
  <img src="/fail-fetch.png" class="w-1/3"/>
</div>

---

# Майстер-клас з багфіксингом

<div class="w-full flex justify-center">
  <div class="ml-20"> 
    <Tweet scale="0.65" id="1917641105245679814" class="w-100"/>
  </div>
</div>

---

# Просто почистимо папку...

<div class="w-full flex justify-center">
  <img src="/fail-clean-directory.png" class="w-4/5"/>
</div>

---

<div class="w-full flex justify-center items-center h-full">
  <div class="w-4/5">
    <h1 class="text-center">Де ми зараз з AI в розробці?</h1>
  </div>
</div>

---
layout: image
image: /vibe-coding-tools.jpg
backgroundSize: contain
---

---
layout: image
image: /current-state-vibe-coding-vs-ai-assisted.png
backgroundSize: contain
---

<!--
https://x.com/mattpocockuk/status/1913313872666321018
-->

---

# Етапи впровадження AI в IT

<div class="w-full flex justify-center">
  <img src="/current-state-0-100.png" class="w-3/5"/>
</div>

---

# Етапи + Інструменти

<div class="w-full flex justify-center">
  <img src="/current-state-0-100-with-icons.png" class="w-3/5"/>
</div>

---

# Інструменти по категоріях

- Загального призначення, генерація документів: ChatGPT, Gemini, Grok, Claude, DeepSeek
- IDE / розширення для IDE: Cursor, Windsurf, Copilot, Cline, Roo Coode, Augment Agent, Trae
- Автономні агенти: Devin, SWE Agent, Open Hands, Devika
- Прототипування / UI: bolt.new, v0.dev, repl.it agent, lovable, same.dev
- MCP: Context7, GitHub, Browser Tools, File System, Git Tools, Figma, Browser Use
- Інструменти/сервіси: Repomix, Task Master, cursor.new

---

# Github Copilot

<div class="w-full flex justify-center">
  <img src="/github-copilot.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://copilot.github.com/">https://copilot.github.com/</a>
</div>

---

# Cursor

<div class="w-full flex justify-center">
  <img src="/cursor.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://www.cursor.com/">https://www.cursor.com/</a>
</div>

---

# Windsurf

<div class="w-full flex justify-center">
  <img src="/windsurf.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://codeium.com/windsurf">https://codeium.com/windsurf</a>
</div>

---

# Cline

<div class="w-full flex justify-center">
  <img src="/cline.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://cline.bot/">https://cline.bot/</a>
</div>

---

# Як це працює: найпростіша генерація коду з LLM

<div class="w-full flex justify-center mt-20">
  <img src="/how-works-prompt-llm-code.png" class="w-4/5"/>
</div>

---

# Промпт складається з компонентів

<div class="w-full flex justify-center mt-20">
  <img src="/how-works-prompt-expanded-llm-code.png" class="w-4/5"/>
</div>

---

# Простий агент

<div class="w-full flex justify-center mt-20">
  <img src="/how-works-simple-agent.png" class="w-4/5"/>
</div>

---

# Агент з інструментами

<div class="w-full flex justify-center mt-20">
  <img src="/how-works-agent-with-tools.png" class="w-4/5"/>
</div>

---

# Агент з інструментами і пам'яттю

<div class="w-full flex justify-center mt-20">
  <img src="/how-works-modern-agent-tools-memory.png" class="w-4/5"/>
</div>

---

# Мультиагентний підхід

<div class="w-full flex justify-center mt-10">
  <img src="/how-works-multi-agent.png" class="w-100"/>
</div>

---

# LLM - моделі для написання коду

<div class="w-full flex justify-center">
  <img src="/lmarena-coding.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://lmarena.ai/">https://lmarena.ai/</a>
</div>

<!--
# SWE Bench Verified

<div class="w-full flex justify-center">
  <img src="/swe-bench.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://www.swebench.com/#verified">https://www.swebench.com/#verified</a>
</div>
-->

---

# Основні проблеми

- Недетермінованість LLM
- Обмеження контекстного вікна
- Неточне слідування інструкціям
- Галюцинації
- Безпека та юридичні питання
- Актуальність знань
- Складнощі з не дуже поширеними технологіями
- ...

---
layout: image-left
image: /butterfly-effect.png
---

# Недетермінованість LLM

Використання LLM для класичного інженера — це як боротьба з хаосом

- **Повторюваність не гарантована**
- **Нестабільні залежності**
- **Розкидані правки по проекту**
- **Масове переписування існуючого коду**
- **Розбіжність (дрейф) агентів у багатоетапних ланцюжках**

---

# Обмеження контекстного вікна

- Поточні моделі обмежені вікном у 128 тис - 10 млн токенів
- З великим контекстом LLM починають галюцинувати
- Запити з великим контекстом працюють повільно
- Запити з великим контекстом коштують дорого
- ...

---

# Скільки токенів займає код?

LOC в токенах LLM

### React:

- **React jsx (100 рядків):** 700 токенів
- **React jsx (200 рядків):** 1,500 токенів

### SQL:

- **SQL скрипт (100 рядків):** 1,150 токенів
- **SQL скрипт (200 рядків):** 2,500 токенів

### Python:

- **Файл Python (100 рядків):** 1,000 токенів
- **Файл Python (200 рядків):** 1,700 токенів

Джерело: https://prompt.16x.engineer/blog/chatgpt-context-window-token-limit

---

# Зростання розміру контекстного вікна з часом

<div class="w-full flex justify-center mt-15">
  <img src="/context-window.png" class="w-3/5"/>
</div>

---

# Але № 1: Ціна

<div class="w-full flex justify-center">
  <img src="/openai-pricing.png" class="w-120"/>
</div>

<div class="w-full flex justify-center mt-5">
  <a href="https://openai.com/api/pricing/">https://openai.com/api/pricing/</a>
</div>

---
layout: image
image: /live-bench.png
backgroundSize: contain
---

# Але № 2: <br> Якість

---

# Але № 3: Швидкість

Оцінка часу виводу 1 млн токенів

<div class="w-full flex justify-center mt-20">
  <img src="/token-output-speed.png" class="w-1/2"/>
</div>

---

# Ризики безпеки та правові аспекти генерації коду ШІ

- Генерація небезпечного (вразливого) коду
- Виконання довільних команд у системі
- Використання інтеграцій із зовнішніми сервісами без належного контролю
- Встановлення небажаних залежностей (вектор атаки)
- Витік конфіденційної інформації та інтелектуальної власності
- Генерація коду, що порушує права інтелектуальної власності

---
layout: section
---

# Рішення

---

# Якою має бути гарна архітектура проєкту <span class="strikethrough-target" v-click.hide>для оптимальної генерації коду</span>?

- **Модульність:** Чіткий поділ на компоненти, низька зв'язність.
- **Чіткі API/Інтерфейси:** Добре визначені контракти між модулями.
- **Підтримуваність:** Читабельний код, тестованість.
- **Консистентність:** Єдині патерни, практики та стиль коду.
- **Автоматизація (CI/CD, Тести):** Автоматизовані процеси збірки, тестування та розгортання.
- **Керування залежностями:** Чітке визначення та керування зовнішніми бібліотеками.
- **Безпека:** Архітектурні рішення + ретельна перевірка згенерованого коду.
- **Документація:** Актуальна документація архітектури та коду.

<style>
.slidev-vclick-target.strikethrough-target {
  /* Ensure it's always visible and doesn't fade */
  opacity: 1 !important;
  pointer-events: auto !important;
  transition: none;
  text-decoration: none; /* Initial state: no strikethrough */
}
.slidev-vclick-target.strikethrough-target.slidev-vclick-hidden {
  /* Apply strikethrough *instead* of hiding when clicked */
  text-decoration: line-through;
  opacity: 1 !important; /* Keep it visible */
  pointer-events: auto !important;
}
</style>

---
layout: image-left
image: /bounded-context.svg
---

# Обмежений контекст (bounded context)

- Концепція з "Domain Driven Design"
- Єдине значення термінів: усі поняття зрозумілі й послідовні тільки всередині цього контексту.
- Ізоляція коду й даних: модель, база, правила та лексикон не змішуються з іншими контекстами.
- Явні інтеграційні контракти: взаємодія ззовні відбувається лише через чітко визначені API / події.

---

# Послідовність розробки

- Генеруємо набір документів
- Прототипуємо
- Розробляємо
- Інтегруємо
- Тестуємо
- Розгортаємо
- ...

---

# Документи

- **Вимоги до проєкту:** Цілі, функції, користувачі (PRD).
- **Критерії приймання:** Умови для перевірки функціональності.
- **Архітектурний дизайн:** Компоненти, технології, потоки даних (ADR).
- **Модель даних:** Схема бази даних, сутності.
- **Специфікації API:** Контракти між модулями.
- **План тестування:** Стратегія та види тестів.
- **Керівництво зі стилю коду:** Правила форматування, лінтинг.
- **Додаткові інструкції для AI:** Шаблони промптів, контекст для AI.

---

# Патерн "Два кроки назад"

<div class="w-full flex justify-center">
  <img src="/two-steps-back.png" class="w-1/5"/>
</div>

---

# Інструменти для промптів репозиторію - Repomix

<div class="w-full flex justify-center">
  <img src="/repomix.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://repomix.com/">https://repomix.com/</a>
</div>

---

# Прототипування

---

# bolt.new

<div class="w-full flex justify-center">
  <img src="/bolt-new.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://bolt.new/">https://bolt.new/</a>
</div>

---

# v0.dev

<div class="w-full flex justify-center">
  <img src="/v0-dev.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://v0.dev/">https://v0.dev/</a>
</div>

---

# repl.it agent

<div class="w-full flex justify-center">
  <img src="/replit.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://repl.it/">https://repl.it/</a>
</div>

---

# MCP - Model Context Protocol

<div class="w-full flex justify-center">
  <img src="/mcp.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://modelcontextprotocol.io/">https://modelcontextprotocol.io/</a>
</div>

---

# Memory bank

---

# MCP.so

<div class="w-full flex justify-center">
  <img src="/mcp-list.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://mcp.so/">https://mcp.so/</a>
</div>

---

<div class="w-full h-full flex justify-center items-center">
  <h1 class="text-center">Поради, хитрощі та ресурси</h1>
</div>

---

# Правила Cursor

<div class="w-full flex justify-center">
  <img src="/cursor-rules.png" class="w-2/3"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://docs.cursor.com/context/rules-for-ai">https://docs.cursor.com/context/rules-for-ai</a>
</div>

---

# Cursor.directory

<div class="w-full flex justify-center">
  <img src="/cursor-directory.png" class="w-4/5"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://cursor.directory/">https://cursor.directory/</a>
</div>

---

# llms.txt

<div class="w-full flex justify-center">
  <img src="/llms-txt.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://llmstxt.org/">https://llmstxt.org/</a>
</div>

---

# Drizzle ORM llms.txt

<Tweet scale="0.65" id="1896981123559002158" class="w-3/4"/>

https://orm.drizzle.team/llms.txt

---

# Режим планування

<div class="w-full flex justify-center">
  <img src="/cursor-plan-mode.png" class="w-1/2"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://forum.cursor.com/t/plan-vs-act-mode-xml-prompt/50996">https://forum.cursor.com/t/plan-vs-act-mode-xml-prompt/50996</a>
</div>

---

# Документування архітектури

https://x.com/flowisgreat/status/1917328733905772880

---

# Пам'ять

https://x.com/elie2222/status/1914374725129666904

---

# Документація

<div class="w-full flex justify-center">
  <img src="/cursor-docs.png" class="w-3/4"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://docs.cursor.com/context/@-symbols/@-docs">https://docs.cursor.com/context/@-symbols/@-docs</a>
</div>

---

# TDD

# Промпт:

## створи ...

## спочатку напиши тести, потім код, потім оновлюй код, доки тести не пройдуть

---

# Плагін Local History

<div class="w-full flex justify-center mt-20">
  <img src="/local-history.png" class="w-1/2"/>
</div>

---

# Ітеративно

<div class="w-full flex justify-center">
  <div class="ml-16"> 
    <Tweet scale="0.55" id="1739052802314539371" class="w-100"/>
  </div>
</div>

---

# Проблеми

- Зміни, що ламають код
- Галюцинації та неправильні рішення
- Дедлоки (взаємні блокування)
- Обмежені знання нових бібліотек/фреймворків
- Проблеми з великими кодовими базами
- Проблеми з безпекою
- Швидкість розробки
- Вартість використання
- ...

---
layout: image-left
image: /vyacheslav-koldovskyy.png
---

# В'ячеслав Колдовський

- К.т.н., доцент
- 20+ років в ІТ
- Менеджер з компетенцій SoftServe Academy
- Сертифікований Google Cloud Professional Architect
- Практикуючий ентузіаст ШІ
- Ютубер: [youtube.com/@programmingmentorua](https://www.youtube.com/@programmingmentorua)
- Блогер: [t.me/programmingmentor](https://t.me/programmingmentor)
- LinkedIn: [koldovsky](https://www.linkedin.com/in/koldovsky/)

---
## layout: end
---

# Дякую!

<div class="flex justify-center w-full h-30 items-center">
  <img src="/slides-qr.png" class="w-25 h-25"/>
</div>

<div class="w-full flex justify-center">
  <a href="https://programmingmentor.github.io/slidev-vibe-coding/">https://programmingmentor.github.io/slidev-vibe-coding/</a>
</div>
