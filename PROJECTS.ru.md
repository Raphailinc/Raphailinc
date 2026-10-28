# Путеводитель по открытому коду

[Профиль](README.ru.md) · [English](PROJECTS.md) · [Инженерные кейсы](case-studies/README.ru.md)

Для знакомства с Python Backend начните с шести закреплённых репозиториев. Код, который можно запустить, и описания самостоятельных проектов доступны отдельно.

## Основные проекты

| Репозиторий | Что проверить |
| :--- | :--- |
| [altpkg-diff](https://github.com/Raphailinc/altpkg-diff/blob/main/README.ru.md) | Python-библиотека и CLI, параллельные запросы, ограниченные повторы и [HTTP-контракт](https://github.com/Raphailinc/altpkg-diff/blob/main/tests/test_api_contract.py). |
| [Task Delay Service](https://github.com/Raphailinc/Task-Delay-Service/blob/main/README.ru.md) | Django/DRF, Celery, часовые пояса и атомарный захват доставки. Начните с `python scripts/demo.py`, затем посмотрите [архитектуру и ограничения](https://github.com/Raphailinc/Task-Delay-Service/blob/main/docs/delivery-design.md) и [сценарии отказов](https://github.com/Raphailinc/Task-Delay-Service/blob/main/api/tests/test_delivery_lifecycle.py). |
| [Pulse](https://github.com/Raphailinc/Pulse/blob/main/README.ru.md) | Flask app factory, авторизация, права на контент и [валидация загрузок](https://github.com/Raphailinc/Pulse/blob/main/tests/test_uploads.py). |
| [Car API](https://github.com/Raphailinc/Car-API/blob/main/README.ru.md) | Marshmallow, уникальность VIN, ответы на ошибки и [API-тесты](https://github.com/Raphailinc/Car-API/blob/main/tests/test_api.py). |
| [Taskboard](https://github.com/Raphailinc/Taskboard/blob/main/README.ru.md) | Django-формы, фильтры, миграции и [доступ к вложениям](https://github.com/Raphailinc/Taskboard/blob/main/myapp/tasks/test_attachments.py). CI проверяет SQLite и PostgreSQL. |
| [Document Detector](https://github.com/Raphailinc/Document-Detector/blob/main/README.ru.md) | Геометрия OpenCV и [синтетические тесты](https://github.com/Raphailinc/Document-Detector/blob/main/tests/test_detector.py). |

## Данные и численные методы

- [Country Parser Toolkit](https://github.com/Raphailinc/Country-Parser-Toolkit/blob/main/README.ru.md) — HTML-парсинг на локальных образцах и нормализация данных.
- [Monte Carlo](https://github.com/Raphailinc/Monte-Carlo/blob/main/README.ru.md) — оценки интегралов и стандартная ошибка.
- [Random Sequence Analysis](https://github.com/Raphailinc/Random-Sequence-Analysis-Toolkit/blob/main/README.ru.md) — выборочные характеристики, повторы и хи-квадрат.
- [Random Variable Distribution](https://github.com/Raphailinc/Random-Variable-Distribution-Toolkit/blob/main/README.ru.md) — преобразование распределения и теоретические частоты.
- [Text Analyser CLI](https://github.com/Raphailinc/text-analyser-cli/blob/main/README.ru.md) — предобработка изображений и интерфейс OCR.
- [Big Data Lab](https://github.com/Raphailinc/Big-Data-Lab/blob/master/README.ru.md) — Scala CLI и расчёты в памяти одного процесса.

## Web и другие языки

- [Mars Lab Project](https://github.com/Raphailinc/Mars-Lab-Project/blob/main/README.ru.md) — Express/MongoDB и формы React.
- [Micro Video Hosting](https://github.com/Raphailinc/Micro-Video-Hosting/blob/main/README.ru.md) — SvelteKit, SQLite и проверка загрузок.
- [vprok parser](https://github.com/Raphailinc/vprok-parser-test-task/blob/main/README.ru.md) — тестовое задание с браузерным сбором и API.
- [ToolOps](https://github.com/Raphailinc/ToolOps/blob/main/README.ru.md) — C++17, предметная модель, TSV и CTest.
- [Dice Duel](https://github.com/Raphailinc/Dice-Duel/blob/main/README.ru.md) — C++17, правила игры и воспроизводимые симуляции.
- [ToDo CLI](https://github.com/Raphailinc/ToDo-CLI/blob/main/README.ru.md) — Java 17, SQLite и JUnit.

## Архив обучения

[2D Net](https://github.com/Raphailinc/2D-Net), [Biomorph Playground](https://github.com/Raphailinc/Biomorph-Playground), [Dragon Curve Playground](https://github.com/Raphailinc/Dragon-Curve-Playground), [RealCross](https://github.com/Raphailinc/RealCross) и [Product Atlas](https://github.com/Raphailinc/Product-Atlas) сохранены как архивные учебные работы. Для оценки текущего backend-кода используйте основной раздел выше.

В README каждого проекта указаны команды запуска и границы проверок. Коммерческий опыт и кейсы самостоятельной разработки описаны в [профиле](README.ru.md).
