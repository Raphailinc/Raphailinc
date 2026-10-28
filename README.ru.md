<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/header-light.svg">
  <img alt="Kamil Velikiy — Python Backend Engineer. FastAPI, Django REST Framework, PostgreSQL. APIs, business systems and integrations." src="assets/header-light.svg" width="1400">
</picture>

[English](README.md) · [Русский](README.ru.md)<br>
[LinkedIn](https://www.linkedin.com/in/kamil-velikiy/) · [Telegram](https://t.me/foreach_dump) · [Резюме на hh.ru](https://obninsk.hh.ru/resume/ca6f82d7ff0cf787bc0039ed1f50714c6a7474)

## Python Backend — API и бизнес-системы

Я Кямиль Великий. Разрабатываю Python API, интеграции и фоновые процессы. **Более двух лет коммерческого backend-опыта**: B2B-порталы для ритейла и MVP мобильного приложения. Основной фокус — целостность данных, явные бизнес-правила, безопасные повторы операций, права доступа и тесты обработки ошибок.

В **«Базис ИТ»** реализовал блокировки операций и восстановление состояния, доработал регистрацию и согласование аккаунтов через Keycloak, расширил API аналитики индексированным поиском и кешированием. В **«Мен Ин Дев»** был единственным backend-разработчиком мобильного MVP: API, модель PostgreSQL, интеграции и поддержка запуска.

Живу в **Москве**. Сейчас занимаюсь самостоятельной проектной разработкой. Рассматриваю удалённые роли **Python Backend** и **Fullstack Python / React**.

**[Инженерные кейсы](case-studies/README.ru.md)** · **[Путеводитель по открытому коду](PROJECTS.md)**

## Инженерные кейсы

Исходные репозитории этих проектов ведутся отдельно. В кейсах разобраны задача, технические решения и границы проверки; тексты кейсов — на английском.

| Проект | Что реализовал | Стек |
| :--- | :--- | :--- |
| **[Sfera](case-studies/sfera.md)** — личная платформа обучения и совместной работы | Пакетное сохранение с проверкой версии, объектные права, история документов, откат импорта и фоновые экспорты | Django/DRF, FastAPI, PostgreSQL, Celery, React/TypeScript |
| **[PDF Label Service](case-studies/pdf-label-service.md)** — локальный MVP выпуска этикеток | Транзакционное резервирование кодов, защита от повторного использования, восстановление после прерванного экспорта | FastAPI, SQLite, pypdf |
| **[AI English Companion](case-studies/ai-english-companion.md)** — Telegram-MVP для практики английского | AI API, учёт использования, платный доступ и защита от повторной обработки платёжных событий | Python, aiogram, SQLite, Pytest |
| **[Ping](case-studies/ping.md)** — напоминания и личное рабочее пространство | Подтверждение перед сохранением, хранение расписания, изоляция данных владельца и инструменты резервного копирования | FastAPI, PostgreSQL, Docker, React/TypeScript |

## Открытый код

Начните с **[altpkg-diff](https://github.com/Raphailinc/altpkg-diff)**, чтобы посмотреть Python-библиотеку и CLI, или с **[Task Delay Service](https://github.com/Raphailinc/Task-Delay-Service)** — Django API и фоновые задачи.

| Репозиторий | На что посмотреть |
| :--- | :--- |
| [altpkg-diff](https://github.com/Raphailinc/altpkg-diff) | Параллельные HTTP-запросы, повторы, сравнение пакетов, отчёты JSON/Markdown и коды выхода CLI |
| [Task Delay Service](https://github.com/Raphailinc/Task-Delay-Service) | DRF-валидация, фильтрация получателей, часовые пояса и Celery |
| [Pulse](https://github.com/Raphailinc/Pulse) | Flask app factory, авторизация, права владельца поста, загрузки и API-тесты |
| [Car API](https://github.com/Raphailinc/Car-API) | Marshmallow, уникальность VIN, CRUD-ошибки и тесты с изолированной БД |
| [Taskboard](https://github.com/Raphailinc/Taskboard) | Django-модели, формы, фильтрация задач и вложения |
| [Document Detector](https://github.com/Raphailinc/Document-Detector) | Контуры OpenCV, перспективное преобразование и тесты на синтетических изображениях |

Это компактные учебные проекты и примеры для портфолио. Запуск, проверки и ограничения описаны в README каждого репозитория.

## Технологии

**Backend:** Python, FastAPI, Django REST Framework, Flask, REST API.<br>
**Данные и задачи:** PostgreSQL, SQL, SQLite, Redis, Celery; Tarantool и Keycloak в коммерческой работе.<br>
**Поставка и проверки:** Docker, Docker Compose, Git, CI/CD, Pytest.<br>
**Интерфейс:** React, TypeScript, JavaScript, интеграция с API и обработка ошибок.

## Образование и связь

ИАТЭ **НИЯУ МИФИ**: бакалавриат «Информационные системы и технологии» (2024), магистратура «Информатика и вычислительная техника» (2026). Обучаюсь в аспирантуре.

По вакансиям, проектам и техническим вопросам: **[Telegram — @foreach_dump](https://t.me/foreach_dump)** или **[LinkedIn](https://www.linkedin.com/in/kamil-velikiy/)**.
