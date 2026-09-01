# Этап 02 — Data Automation

## Цель
Перейти от одноразового скрипта к полезной автоматизации: несколько источников → нормализация → валидация → БД → фильтры → уведомления.

## Итоговый проект
Monitoring & Notification Service: регулярно проверять источники, находить новые/изменившиеся объекты, хранить историю и отправлять подходящие результаты в Telegram.

## Стек
Python, httpx, BeautifulSoup, Pydantic, SQLAlchemy, PostgreSQL, pytest, logging, Telegram Bot API, cron.

## Изучить
HTTP: methods, status codes, headers, cookies, timeouts, retries, pagination, rate limits, JSON APIs.

Данные: отделять сырой внешний формат от валидированной модели, внутренней бизнес-модели и хранения.

PostgreSQL: tables, keys, SELECT/INSERT/UPDATE, JOIN, indexes, transactions, constraints.

Automation: periodic execution, idempotency, retries, deduplication, state, logging.

## Процесс
1. Один источник.
2. Определить внутреннюю модель.
3. Сохранить данные и историю в PostgreSQL.
4. Добавить второй источник.
5. Вынести фильтры в тестируемую бизнес-логику.
6. Добавить уведомления без повторного спама.
7. Запускать по расписанию.

## Коммерческая связь
После этого этапа можно пробовать маленькие задачи: сбор данных, мониторинг, отчёты, CSV/JSON processing, уведомления и простые API-интеграции.

## Definition of Done
- [ ] минимум 2 источника;
- [ ] PostgreSQL;
- [ ] Pydantic validation;
- [ ] type hints;
- [ ] deduplication;
- [ ] retries/timeouts;
- [ ] logging;
- [ ] automatic execution;
- [ ] Telegram/email notification;
- [ ] tests основной логики;
- [ ] README;
- [ ] срок около 2–3 недель.

## Не делать
Redis, Celery, Kubernetes, микросервисы и сложный dashboard без реальной необходимости.

## Переход
Ты умеешь хранить состояние и объяснить поведение системы при timeout, повторном запуске и уже обработанном объекте.
