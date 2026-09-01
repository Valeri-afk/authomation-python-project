# Этап 04 — FastAPI и Web Service

## Цель
Превратить automation-логику в backend-сервис. Это возвращает знакомую модель Node.js/React, но backend пишется на Python.

## Архитектура
Browser/React → FastAPI → application logic → PostgreSQL / automation → external APIs/sites.

## Стек
Backend: Python, FastAPI, Pydantic, SQLAlchemy, PostgreSQL, pytest, httpx.

Frontend: React + TypeScript. Использовать уже имеющийся опыт, а не изучать frontend заново.

## Изучить
- HTTP request/response;
- routing;
- path/query/body parameters;
- validation;
- status codes;
- FastAPI dependencies;
- database sessions;
- authentication/authorization basics;
- CORS;
- OpenAPI;
- background jobs.

## Процесс
1. Сначала API без frontend: POST/GET/DELETE для automation jobs.
2. Подключить PostgreSQL и migrations.
3. Подключить существующий automation engine.
4. Добавить authentication.
5. Добавить минимальный React dashboard.

Архитектурное правило: route → service/use case → repository/external adapter.

Не превращать проект в enterprise-архитектуру из десятков слоёв.

## Definition of Done
- [ ] FastAPI;
- [ ] CRUD/API automation jobs;
- [ ] Pydantic schemas;
- [ ] PostgreSQL;
- [ ] authentication;
- [ ] background execution;
- [ ] API tests;
- [ ] OpenAPI;
- [ ] минимальный React dashboard;
- [ ] понятный README.

## Переход
Уметь объяснить путь запроса от браузера до БД/automation worker и воспроизводимо запускать сервис локально.
