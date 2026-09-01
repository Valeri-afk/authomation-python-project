# Этап 03 — Browser Automation

## Цель
Научиться автоматизировать разрешённые процессы, где нет удобного API и приходится взаимодействовать с web-приложением через браузер.

## Итоговый проект
Демонстрационный workflow на тестовом или собственном сайте: Python → Playwright → browser → login/navigation/form → download → processing → result.

## Стек
Python, Playwright, pytest, Pydantic и automation core из этапа 02.

## Изучить
- browser contexts;
- pages;
- selectors;
- forms;
- navigation;
- downloads;
- screenshots/traces;
- waits и page states;
- cookies/sessions;
- timeouts;
- retry strategy.

Предпочитать устойчивые DOM selectors вместо координат мыши.

## Процесс
1. Использовать собственный/тестовый сайт.
2. Реализовать один workflow.
3. Обработать missing elements, медленный сайт, failed login и failed download.
4. Отделить browser layer от business logic.
5. Тестировать бизнес-логику без браузера.

## Ограничения
Автоматизировать только сервисы и процессы, где это разрешено правилами. Не строить услугу вокруг обхода CAPTCHA, антибот-защит, rate limits, paywalls, DRM или иных технических ограничений.

## Коммерческая связь
Подходящие классы задач: регулярный экспорт, разрешённое заполнение форм, работа с личными кабинетами клиента, отчёты, QA/testing workflows и интеграции без API.

## Definition of Done
- [ ] законченный browser workflow;
- [ ] устойчивые selectors;
- [ ] timeout/error handling;
- [ ] screenshots/traces;
- [ ] browser layer отделён;
- [ ] tests бизнес-логики;
- [ ] README;
- [ ] срок около 1–2 недель.

## Переход
Понимать разницу между automation engine и интерфейсом управления им. Следующий этап — HTTP API.
