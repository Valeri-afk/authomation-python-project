# Python Automation Roadmap

Практический маршрут от текущего опыта программирования к первым оплачиваемым automation-задачам и далее к backend/software engineering.

## Что проверено рынком

В российском freelance-сегменте регулярно встречаются заказы и услуги на стыке Python, парсинга, API, CSV/Excel, Playwright, PostgreSQL, Telegram, Docker и автоматизации. Есть как очень дешёвые простые задачи, так и более дорогие сервисы с API, очередями, БД и deployment. Поэтому roadmap построен не вокруг абстрактного «изучения Python», а вокруг последовательного освоения именно этого набора компетенций. 

Примеры наблюдаемых форматов задач: Python-скрипты автоматизации и интеграций API; сбор данных и мониторинг; Playwright/browser automation; FastAPI + PostgreSQL + Docker; фоновые задачи и очереди. 

## Конечная цель

Уметь взять небольшую реальную задачу:

`внешний источник → получение данных → validation → processing → storage/API → автоматическое действие`

и самостоятельно довести её до работающего, документированного и воспроизводимого результата.

После этого возможны два параллельных пути:

- небольшие оплачиваемые automation/integration задачи;
- переход в Junior Python/Backend/Automation/Software Engineer позицию.

## Roadmap

| Этап | Что проверяем на рынке | Результат |
|---|---|---|
| 01 | Python scripts, API, parsing, file processing | небольшой CLI/tool |
| 02 | scraping, monitoring, data processing, notifications | automation service |
| 03 | browser automation | Playwright workflow |
| 04 | backend/API integration | FastAPI service + web UI |
| 05 | deployment/support | Linux + Docker + VPS |
| 06 | коммерческое применение | первая оплачиваемая задача + портфолио |

## Главный принцип

**CLI — это стартовый интерфейс, а не профессия.** После проверки внутренней логики инструмент может остаться CLI, работать в фоне или получить web/desktop интерфейс. UI добавляется тогда, когда он нужен пользователю.

Второй принцип: **не пытаться конкурировать с senior-разработчиком на рынке «Python developer».** Вместо этого постепенно становиться специалистом по конкретным автоматизируемым процессам: data collection, API integration, monitoring, document/file processing, browser automation и workflow automation.

## Definition of Done всего маршрута

- Python и type hints;
- работа с HTTP/API;
- parsing и browser automation;
- PostgreSQL;
- FastAPI;
- background jobs/scheduling;
- тесты и logging;
- Linux/Docker/VPS;
- один законченный automation-проект;
- минимум одна попытка применения навыков к реальной задаче.

## Документы

- [Этап 01 — Python и CLI](roadmap/01-python-cli.md)
- [Этап 02 — Data Automation](roadmap/02-data-automation.md)
- [Этап 03 — Browser Automation](roadmap/03-browser-automation.md)
- [Этап 04 — FastAPI и Web Service](roadmap/04-fastapi-service.md)
- [Этап 05 — Production-like Deployment](roadmap/05-production-deployment.md)
- [Этап 06 — Первый заработок](roadmap/06-first-income.md)

## Вне roadmap на первых этапах

Не тратить время на Kubernetes, микросервисы, собственные framework/ORM, сложный DevOps и высоконагруженную архитектуру до появления реальной задачи, которая этого требует.
