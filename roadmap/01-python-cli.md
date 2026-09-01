# Этап 01 — Python и CLI

## Цель
Научиться использовать Python как быстрый прикладной инструмент. Критерий завершения: самостоятельно написать небольшую программу input → processing → output, разбить её на модули, обработать ошибки и проверить типы.

## Итоговый проект
CLI-инструмент: список URL → HTTP → извлечение данных → JSON/CSV.

## Стек
- Python 3.x
- httpx
- beautifulsoup4
- argparse
- pytest
- Ruff
- Pyright
- Git

## Изучить
- переменные, условия, циклы;
- функции;
- list, dict, set, tuple;
- comprehensions;
- exceptions;
- modules/packages;
- venv и pip;
- pathlib;
- JSON/CSV;
- базовое ООП;
- type hints.

С самого начала используй type hints и Pyright: это даст привычную после C++ статическую проверку.

## Процесс
1. URL → HTTP GET → print.
2. Извлечь конкретное поле.
3. Добавить несколько источников.
4. Добавить CLI: input, output, filter, help.
5. Типизировать публичные функции.
6. Добавить тесты parsing/filtering на сохранённых данных.
7. Добавить timeout, HTTP errors и понятные ошибки ввода.

## Definition of Done
- [ ] отдельный venv;
- [ ] README;
- [ ] CLI с help;
- [ ] type hints;
- [ ] Pyright/Ruff проходят;
- [ ] pytest для основной логики;
- [ ] JSON или CSV output;
- [ ] проект закончен за 7–10 дней.

## Не делать
Не писать собственный HTTP client, parser framework, GUI, FastAPI, PostgreSQL или Docker.

## Переход
Ты готов, когда можешь взять небольшую незнакомую задачу, найти документацию/библиотеку и получить рабочий результат без пошагового tutorial.
