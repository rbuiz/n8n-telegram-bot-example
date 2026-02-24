# n8n-telegram-bot-example

🤖 Пример Telegram бота на n8n с искусственным интеллектом. Бот выступает в роли консультанта и помогает подбирать курсы (на примере школы выпечки блинов). Показывает интеграцию Telegram + OpenAI, работу с памятью диалогов и системным промптом. Используйте как шаблон для своих проектов — просто замените промпт и каталог!

<div align="center">
  <img src="https://img.shields.io/badge/n8n-example-blue?style=for-the-badge&logo=n8n" alt="n8n">
  <img src="https://img.shields.io/badge/Telegram-Bot-26A5E4?style=for-the-badge&logo=telegram" alt="Telegram">
  <img src="https://img.shields.io/badge/OpenAI-Integration-412991?style=for-the-badge&logo=openai" alt="OpenAI">
</div>

---

## 📋 О проекте

Этот репозиторий содержит готовый шаблон n8n workflow для создания Telegram бота с AI-агентом. Бот помогает пользователям подобрать идеальный курс по выпечке блинов, учитывая их уровень подготовки и цели.

### ✨ Возможности

- 🧠 **AI диалоги** — использует OpenAI GPT
- 📊 **Определение уровня** — от новичка до профи
- 🎯 **Выявление целевых клиентов** — кто готов купить
- 📚 **Рекомендации курсов** — из 5 программ
- 💬 **Работа с возражениями** — о цене и сложности
- 🧠 **Память диалога** — помнит контекст

---

## 🗺️ Структура

![n8n Workflow Preview](n8n-workflow-preview.jpg)

### Компоненты:

| Узел | Назначение |
|------|------------|
| **Telegram Trigger** | Получает сообщения от пользователей |
| **AI Agent** | Основной мозг бота с системным промптом |
| **Simple Memory** | Хранит историю диалога (20 сообщений) |
| **OpenAI Chat Model** | Подключает языковую модель GPT |
| **Send Message** | Отправляет ответ обратно в Telegram |

---

## 📦 Артефакты проекта

| Файл | Назначение |
|------|------------|
| **📄 Workflow** | |
| [`n8n_telegram_ai_template.json`](n8n_telegram_ai_template.json) | Основной workflow для n8n |
| **📄 Документация** | |
| [`system_prompt.txt`](system_prompt.txt) | Системный промпт для AI Agent |
| **🖼️ Изображения** | |
| [`n8n-workflow-preview.jpg`](n8n-workflow-preview.jpg) | Скриншот структуры workflow |
| [`bot-conversation-example.jpg`](bot-conversation-example.jpg) | Пример диалога с ботом |

---

## 📁 Каталог курсов (пример)

| Курс | Уровень | Уроков | Цена |
|------|---------|--------|------|
| 🥞 Идеальный первый блин | Начинающий | 4 | 1990 ₽ |
| 🥛 Блины на кислом молоке | Начинающий+ | 5 | 2490 ₽ |
| 🌾 Блины без глютена | Средний | 6 | 2990 ₽ |
| 🎨 Блинные кружева | Продвинутый | 4 | 2790 ₽ |
| 🔥 Французские крепы | Эксперт | 7 | 3490 ₽ |

---

## 🚀 Быстрый старт

### Требования
- Аккаунт [Amvera](https://cloud.amvera.ru/)
- Telegram бот (через [@BotFather](https://t.me/botfather))
- API ключ [OpenAI](https://platform.openai.com/)

### Установка

1. **Импортируйте в n8n**
   - Откройте n8n
   - Нажмите **Import from File**
   - Выберите файл [`n8n_telegram_ai_template.json`](n8n_telegram_ai_template.json)

2. **Настройте учетные данные**
   - **Telegram**: добавьте токен бота
   - **OpenAI**: добавьте API ключ

3. **Замените системный промпт**
   - В узле **AI Agent** найдите `YOUR_SYSTEM_PROMPT_HERE`
   - Вставьте свой текст

4. **Активируйте workflow**
   - Нажмите кнопку **Active** в правом верхнем углу

5. **Пишите своему боту в Telegram!** 🎉

---

## 🛠️ Адаптация под свой проект

1. Откройте узел **AI Agent**
2. Найдите поле `systemMessage`
3. Замените промпт на свой.
Можете взять наш системный промпт - [`system_prompt.txt`](system_prompt.txt), как пример, и отредактировать под свои нужды.
4. Готово!

---

## 🔒 Безопасность

Все чувствительные данные заменены плейсхолдерами:

| Плейсхолдер | Описание |
|-------------|----------|
| `YOUR_TELEGRAM_CREDENTIAL_ID` | ID учетных данных Telegram |
| `YOUR_OPENAI_CREDENTIAL_ID` | ID учетных данных OpenAI |
| `YOUR_WEBHOOK_ID` | ID вебхука |
| `YOUR_SYSTEM_PROMPT_HERE` | Ваш системный промпт |

**Никогда не публикуйте реальные токены!**

## 💬 Пример диалога

*Как бот помогает подобрать курс*

![Пример диалога с ботом](bot-conversation-example.jpg)


### Особенности диалога:
- ✅ Бот общается тепло, с эмодзи
- ✅ Задает уточняющие вопросы
- ✅ Не навязывает, а помогает выбрать
- ✅ Работает с возражениями

---

## ⭐ Поддержка

Если проект полезен — поставьте звезду на GitHub! ⭐

---

<div align="center">
  <a href="https://github.com/yourusername/n8n-telegram-bot-example">🔗 GitHub</a>
  •
  <a href="https://t.me/yourusername">📬 Telegram</a>
  •
  <a href="https://forum.n8n.io/">💬 n8n Community</a>
</div>



