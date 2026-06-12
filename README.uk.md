# Антигравітаційний стартер 🛰️

<div align="center">
  <a href="README.md">English</a> | <a href="README.id.md">Bahasa Indonesia</a> | <a href="README.zh.md">简体中文</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.fr-ca.md">Français (CA)</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt-br.md">Português (BR)</a> | <a href="README.vi.md">Tiếng Việt</a> | <a href="README.pl.md">Polski</a> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.tr.md">Türkçe</a> | <a href="README.it.md">Italiano</a> | <a href="README.ru.md">Русский</a> | <strong>Українська</strong> | <a href="README.nl.md">Nederlands</a>
</div>

<br />

<div align="center">
  <h3><strong>AI Агенти неймовірно розумні. Але вони сліпі в безладному робочому просторі.</strong></h3>
  <p><strong>Antigravity Starter — це незаймана пісочниця Next.js 16, створена на основі штучного інтелекту, яка надає вашим редакторам штучного інтелекту ідеальне бачення.</strong></p>

  <p>Припиніть витрачати токени, страждати від галюцинацій ШІ та боротися з безладною структурою папок. Кодування за допомогою штучного інтелекту має відчуватися як магія, і тепер це так.</p>
</div>

> 📦 Безкоштовний шаблон від **andiupn** ([kuncimu.com](https://kuncimu.com)) · Ліцензовано відповідно до [ліцензії MIT](LICENSE)  
> ☕ Якщо це корисно, [пригости мене кавою](https://ko-fi.com/andiupn) · 🚀 Потрібне монорепо для кількох проектів із першим статусом? Спробуйте [PRO версію](https://github.com/sponsors/andiupn?frequency=monthly)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub release](https://img.shields.io/github/v/release/andiupn/antigravity-starter)](https://github.com/andiupn/antigravity-starter/releases)
[![Ko-Fi](https://img.shields.io/badge/Ko--fi-Support-ff5f5f?logo=ko-fi)](https://ko-fi.com/andiupn)
[![Patreon](https://img.shields.io/badge/Patreon-Support-f96854?logo=patreon)](https://patreon.com/AndiUpn)
[![Trakteer](https://img.shields.io/badge/Trakteer-Support-red?logo=trakteer)](https://trakteer.id/andi_upn/gift)
[![Saweria](https://img.shields.io/badge/Saweria-Support-yellow?logo=saweria)](https://saweria.co/andiupn)

---

## 💡 Проблема: чому традиційні робочі простори зазнають невдачі ШІ
Агенти ШІ (Курсор, Близнюки, Клод) мають феноменальні можливості. Але коли їх опускають у стандартні захаращені каталоги, вони губляться. Вони читають невідповідні папки, продувають ваш бюджет токенів, галюцинують і розміщують файли не в тих каталогах, оскільки немає чітких меж.

---

## ⚡ Рішення: три стовпи першокласних риштувань AI

### 1. 🛰️ Perfect Vision для AI (AI-First Layout)
Ми розробили кожну папку, конфігурацію та правило `.gitignore`, щоб діяти як дорожні карти для вашого ШІ. Робочий простір надзвичайно чистий, що дозволяє Cursor або Gemini зрозуміти всю вашу архітектуру **Next.js 16 + React 19 + Tailwind v4** менш ніж за 3 секунди. Нуль марних жетонів, максимальна точність.

### 2. 🤖 Спеціалізована команда, а не звичайний чат-бот
Ви не розмовляєте з порожньою коробкою ШІ. Ви отримуєте команду з 2 попередньо налаштованих вузькоспеціалізованих автономних агентів ШІ:
- **`@code-reviewer`** — Ваша ретельна, сувора команда контролю якості, яка перевіряє якість коду, лінси та структуру перед фіксацією.
- **`@research-assistant`** — високошвидкісний, економічно ефективний дослідницький агент, призначений для безпечного вивчення нових документів і бібліотек API.

### 3. ⚡ Навички в один клік (робочі процеси)
Виконуйте складні робочі процеси розробки за допомогою простих команд. Оснащений 8 автоматизованими робочими процесами для багаторазового використання (`/skills`), які перетворюють ручне створення скелетів, перевірку середовища та написання тестів у завдання за 1 секунду.

---

## 📊 LITE vs PRO: преміум-оновлення

| Що ви можете зробити | 🆓 LITE (безкоштовно) | 💎 PRO (Платно) |
|---|:---:|:---:|
| **Спеціалізовані агенти** | 2 | 5 (+планувальник, архітектура, охорона) |
| **Навички робочого процесу** | 8 | 23 (+ Drizzle sync, Docker, rules-audit тощо) |
| **Структура робочого простору** | Простий (`src/`, `docs/`) | Перший статус Monorepo (`active/`, `staging/` тощо) |
| **Ops Ready Config** | ❌ | ✅ (Docker Compose, Caddyfile) |
| **Налаштування проекту** | 1 (Далі.js) | 4 (Наступна програма, SPA, Laravel, Flutter) |

👉 **[Переглянути повний посібник із порівняння функцій і оновлення](COMPARISON.md)**

---

## 📂 План робочого простору

```
your-workspace/
  .gemini/             # AI agent configs, automation skills, and wiki
  docs/                # Pristine research and implementation plans
  src/                 # Main directory for your application source code
  .env.example         # Template for environment variables
  .gitignore           # Standard Git ignore file
  .mcp.json            # Model Context Protocol (MCP) configuration
  GEMINI.md            # AI coding rules & workspace guidelines
  LICENSE              # Project license (MIT License)
```

---

## 🚀 Розпочніть у 3 кроки

### 1. Скопіюйте конфігурації:

```bash
cp .env.example .env
```

*(Вставте свій `GITHUB_TOKEN`, щоб увімкнути інтеграцію репозиторію).*

### 2. Налаштуйте дозволи AI:

```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```

*(Розкоментуйте та встановіть `permissions` відповідно до вашої ОС).*

### 3. Почніть кодування:
Відкрийте цей робочий простір у своєму улюбленому редакторі з підтримкою штучного інтелекту та відчуйте швидкість.

---

## 💖 Підтримайте цей проект (пожертви)

Якщо цей шаблон прискорив ваш робочий процес кодування, подумайте про підтримку:
- **Ko-fi:** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon:** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **Trakteer:** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **Saweria:** [saweria.co/andiupn](https://saweria.co/andiupn)

---

## 📄 Ліцензія

Цей проект ліцензований згідно з **ліцензією MIT**. Додаткову інформацію див. у файлі [LICENSE](LICENSE).