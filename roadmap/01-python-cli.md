# Этап 01 — Python + прикладные инструменты

## Цель
Не «выучить Python», а научиться быстро решать небольшие прикладные задачи: получить данные, обработать их, сохранить или передать дальше.

CLI здесь только интерфейс для разработки и отладки. Коммерческая ценность — в автоматизации, а не в командной строке.

## Что проверяем на рынке
Типовые входные задачи: Python-скрипт, работа с API, parsing HTML/JSON, CSV/Excel processing, преобразование данных, небольшая интеграция.

## Итоговый проект
Сделать `data-tool`:

`URL/API/CSV → validation → filtering/transformation → JSON/CSV report`

Поддержать как минимум два источника: REST API и HTML-страницу.

## Среда разработки

Установить:

- Python 3.x;
- VS Code;
- VS Code extensions: **Python (Microsoft)**, **Pylance (Microsoft)**, **Ruff (Astral)**;
- Git.

В репозитории уже лежат `.vscode/extensions.json` и `.vscode/settings.json`, поэтому проект сам рекомендует extensions и базовые настройки.

Важно различать уровни:

- `httpx`, `beautifulsoup4`, `pydantic`, `pytest` — Python-пакеты;
- Ruff — CLI-инструмент lint/format и VS Code extension;
- Pylance — редакторный анализ типов на базе Pyright;
- Git — система контроля версий;
- Python — интерпретатор, отдельный от VS Code extension.

## Стек
- Python 3.x
- httpx
- BeautifulSoup
- Pydantic
- argparse
- pytest
- Ruff
- Pyright/Pylance
- Git

## Изучить
- функции и модули;
- list/dict/set/tuple;
- comprehensions;
- exceptions;
- pathlib;
- JSON/CSV;
- venv/pip;
- `pyproject.toml`;
- type hints;
- dataclasses/Pydantic;
- базовое ООП;
- чтение документации библиотек.

## Ключевой навык этапа
**Не писать всё самому.** Получив задачу, сначала определить, есть ли библиотека/API, который уже решает часть проблемы.

Тренировать цикл:

`задача → поиск документации → выбор библиотеки → маленький прототип → реализация`

## Процесс
1. Создать `.venv`.
2. Описать проект и зависимости через `pyproject.toml`.
3. Настроить VS Code/Pylance/Ruff.
4. Получить данные из REST API.
5. Валидировать их Pydantic-моделью.
6. Получить данные из HTML.
7. Привести оба источника к единой внутренней модели.
8. Фильтровать и преобразовывать.
9. Сохранить JSON/CSV.
10. Добавить CLI для параметров.
11. Добавить tests, type checking и error handling.

## Definition of Done
- [ ] `.venv` используется локально;
- [ ] `pyproject.toml` содержит метаданные и зависимости проекта;
- [ ] два разных источника;
- [ ] единая внутренняя модель данных;
- [ ] type hints;
- [ ] Pydantic validation;
- [ ] HTTP timeout/error handling;
- [ ] pytest для бизнес-логики;
- [ ] Pyright/Pylance без существенных type errors;
- [ ] Ruff check/format;
- [ ] README;
- [ ] проект завершён примерно за 7–10 дней.

## Не делать
Не писать собственный framework, HTTP client, parser, GUI, FastAPI или сложную архитектуру.

Не изучать весь Python перед началом проекта. Сначала решить задачу, а синтаксис и библиотеку изучать по мере необходимости.

## Коммерческий порог
После этого этапа можно пробовать самые маленькие задачи, если они ограничены по scope: преобразование файлов, API integration, простой сбор данных, отчёт или скрипт.

## Переход
Ты способен взять неизвестный API/формат данных, разобраться по документации и за несколько часов сделать маленький proof of concept.
