# Pavel

[English](#english) · [Русский](#русский)

---

## English

I build Telegram bots, backends and automation that work with real data, and deploy them on infrastructure that is closed to the public internet. Open to freelance projects.

### What I can do for you

- **Telegram bots with admin panels and AI.** Order intake, validation, AI analysis of requests, admin notifications and a web admin panel. Stack: aiogram, FastAPI, PostgreSQL, React.
- **Parsers and data collection.** Real-time and scheduled collection from exchanges and web sources, cleaned and stored for use.
- **Automation with n8n.** Multi-step scenarios and data orchestration on a self-hosted n8n, connected to bots, APIs and databases.
- **Secure deployment.** A hardened VPS with no publicly exposed management panels: private access over Tailscale, key-only SSH and CrowdSec intrusion prevention.

### Selected work

**[vkat_py](https://github.com/ascezis/vkat_py)**: offline Python trainer for a programming school. Students who join a course late have to catch up with the group; vkat_py lets them practise at their own pace and checks every solution by actually running it. Real Python in the browser (Pyodide / WebAssembly), no internet required. In production; 30+ students have used it in real classes. Vanilla JavaScript, no build step.

**[asc_prod_bot](https://github.com/ascezis/asc_prod_bot)**: Telegram bot that takes video-editing orders end to end. It validates the request, has an AI model assess budget, timeline and risks, notifies the admin and stores everything in PostgreSQL. Comes with a React admin panel and an Electron launcher.

**SHADOW / TANK**: hardened infrastructure for self-hosted automation (n8n) and container management (Portainer), in four layers:
- a private Tailscale network, so management panels are unreachable from the public internet;
- CrowdSec analysing SSH and Docker logs and blocking attackers at the firewall;
- key-only SSH on a non-standard port, with root access locked down and monitored by a small Python daemon;
- disk limits, log rotation and automatic clean-up to keep the server stable.

**[NyxD](https://github.com/ascezis/NyxD)**: private, offline-first encrypted diary for Android. Argon2id key derivation, SQLCipher, no key stored on disk. The repository documents its threat model and known limitations openly, including why Android Keystore was deliberately not used.

Also: [BeholderEyes](https://github.com/ascezis/BeholderEyes), a desktop toolkit for D&D 5e game masters (Electron, React, TypeScript, SQLite).

### How I work

- I state what a system protects against and what it does not.
- I document architecture and setup, so a project can be handed over and maintained by someone else.
- I keep the exposed surface small: secrets stay out of repositories, management access goes through private channels only.

### Stack

- **Backend:** Python, aiogram, FastAPI, SQLAlchemy, PostgreSQL, aiohttp
- **Automation:** n8n, parsers, AI API integrations
- **Frontend and desktop:** JavaScript, TypeScript, React, Electron
- **Mobile:** Dart, Flutter
- **Infrastructure and security:** Debian, Docker, Docker Compose, Portainer, Tailscale, CrowdSec, SSH hardening, Argon2id, SQLCipher

### Contact

Telegram: [@crackedmachines](https://t.me/crackedmachines). In your first message, please tell me what you need built, the deadline and a rough budget.

---

## Русский

Делаю Telegram-ботов, бэкенды и автоматизацию, которые работают с реальными данными, и разворачиваю их на инфраструктуре, закрытой от публичного интернета. Открыт для заказов.

### Чем могу помочь

- **Telegram-боты с админ-панелью и AI.** Приём заявок, проверка данных, AI-анализ, уведомления администратору и веб-панель управления. Стек: aiogram, FastAPI, PostgreSQL, React.
- **Парсеры и сбор данных.** Сбор данных с бирж и сайтов в реальном времени или по расписанию, очистка и сохранение в удобном для работы виде.
- **Автоматизация на n8n.** Сложные многошаговые сценарии и оркестрация данных на self-hosted n8n, связанные с ботами, API и базами данных.
- **Безопасный деплой.** Укреплённый VPS, у которого панели управления не выставлены в публичный интернет: закрытый доступ через Tailscale, вход по SSH-ключам и защита от вторжений CrowdSec.

### Избранные работы

**[vkat_py](https://github.com/ascezis/vkat_py)**: офлайн-тренажёр по Python для школы программирования. Ученик, который пришёл в группу позже остальных, может догнать программу в своём темпе, а каждое решение проверяется реальным запуском кода. Настоящий Python работает прямо в браузере (Pyodide / WebAssembly) и не требует интернета. Проект в эксплуатации: на занятиях его опробовали более 30 учеников. Чистый JavaScript, без сборки.

**[asc_prod_bot](https://github.com/ascezis/asc_prod_bot)**: Telegram-бот, который принимает заявки на видеомонтаж от начала до конца. Проверяет данные, просит AI-модель оценить бюджет, сроки и риски, уведомляет администратора и сохраняет всё в PostgreSQL. К нему прилагаются админ-панель на React и Electron-лаунчер.

**SHADOW / TANK**: укреплённая инфраструктура для self-hosted автоматизации (n8n) и управления контейнерами (Portainer), четыре уровня защиты:
- закрытая сеть Tailscale, благодаря которой панели управления недоступны из публичного интернета;
- CrowdSec анализирует логи SSH и Docker и блокирует злоумышленников на уровне файрвола;
- вход по SSH только по ключам, на нестандартном порту; root-доступ закрыт и находится под наблюдением небольшого демона на Python;
- лимиты диска, ротация логов и автоматическая очистка, чтобы сервер работал стабильно.

**[NyxD](https://github.com/ascezis/NyxD)**: приватный офлайн-дневник с шифрованием для Android. Ключ выводится через Argon2id, база хранится в SQLCipher, сам ключ на диск не записывается. В репозитории открыто описана модель угроз и известные ограничения, в том числе почему Android Keystore сознательно не используется.

Также: [BeholderEyes](https://github.com/ascezis/BeholderEyes), настольный инструмент для мастеров D&D 5e (Electron, React, TypeScript, SQLite).

### Как я работаю

- Прямо пишу, от чего система защищает, а от чего нет.
- Документирую архитектуру и запуск, чтобы проект можно было передать и поддерживать без меня.
- Держу поверхность атаки небольшой: секреты не попадают в репозитории, доступ к управлению идёт только по закрытым каналам.

### Стек

- **Бэкенд:** Python, aiogram, FastAPI, SQLAlchemy, PostgreSQL, aiohttp
- **Автоматизация:** n8n, парсеры, интеграции с AI API
- **Фронтенд и десктоп:** JavaScript, TypeScript, React, Electron
- **Мобильная разработка:** Dart, Flutter
- **Инфраструктура и безопасность:** Debian, Docker, Docker Compose, Portainer, Tailscale, CrowdSec, харденинг SSH, Argon2id, SQLCipher

### Связь

Telegram: [@crackedmachines](https://t.me/crackedmachines). В первом сообщении, пожалуйста, напишите, что нужно сделать, желаемые сроки и примерный бюджет.
