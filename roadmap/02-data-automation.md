# Этап 02 — Data Automation

## Цель
Перейти от одноразового скрипта к полезной автоматизации: источник → получение → validation → processing → storage → action.

## Что проверяем на рынке
Это основной практический слой маршрута. Здесь встречаются задачи по сбору данных, API integrations, мониторингу, отчётам, CSV/JSON processing, уведомлениям и регулярному запуску.

## Итоговый проект
**Monitoring & Notification Service.** Регулярно проверять несколько источников, находить новые/изменившиеся объекты, хранить историю, фильтровать и отправлять подходящие результаты.

Сделать минимум две интеграции:
- REST API;
- HTML source или CSV/file source.

## Стек
Python, httpx, BeautifulSoup, Pydantic, SQLAlchemy, PostgreSQL, pytest, logging, Telegram Bot API, cron.

## Изучить
HTTP: methods, status codes, headers, cookies, timeouts, retries, pagination, rate limits, JSON APIs.

Данные: raw input → validated model → business model → storage/output.

PostgreSQL: tables, keys, SELECT/INSERT/UPDATE, JOIN, indexes, transactions, constraints.

Automation: periodic execution, idempotency, retries, deduplication, state, logging.

## Ключевой навык
**Исследование чужой системы.** Перед реализацией определить:

1. есть ли API;
2. какая документация существует;
3. какие ограничения и rate limits есть;
4. какой минимальный набор данных нужен;
5. что является уникальным идентификатором объекта;
6. что должно происходить при повторном запуске.

Это ближе к реальной коммерческой работе, чем знание конкретной библиотеки.

## Процесс
1. Один источник.
2. Сделать collector с понятным интерфейсом.
3. Определить внутреннюю модель.
4. Сохранить данные и историю в PostgreSQL.
5. Добавить второй источник через отдельный adapter.
6. Вынести фильтры в тестируемую бизнес-логику.
7. Добавить deduplication.
8. Добавить уведомления без повторного спама.
9. Запускать по расписанию.
10. Проверить поведение при timeout, повторном запуске и недоступном источнике.

## Коммерческий порог
**После этого этапа уже начинать искать маленькие реальные задачи.** Не ждать окончания всего roadmap.

Подходящие первые категории:
- API integration;
- сбор данных;
- CSV/Excel/JSON processing;
- простые мониторинги;
- регулярные отчёты;
- уведомления;
- небольшие внутренние automation scripts.

## Definition of Done
- [ ] минимум 2 источника;
- [ ] PostgreSQL;
- [ ] Pydantic validation;
- [ ] type hints;
- [ ] deduplication;
- [ ] retries/timeouts;
- [ ] logging;
- [ ] automatic execution;
- [ ] notification;
- [ ] tests основной логики;
- [ ] README с архитектурой;
- [ ] срок около 2–3 недель.

## Не делать
Не добавлять Redis, Celery, Kubernetes, микросервисы или сложный dashboard только ради «правильного стека». Они появятся тогда, когда конкретная задача действительно требует их.

## Переход
Ты умеешь взять неизвестный источник, исследовать его, получить данные, привести их к собственной модели, сохранить состояние и безопасно повторять процесс.
