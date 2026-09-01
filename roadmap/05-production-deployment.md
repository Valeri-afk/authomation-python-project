# Этап 05 — Production-like Deployment

## Цель
Перестать считать «работает на моём компьютере» завершённым состоянием. Научиться запускать сервис в Linux и диагностировать его без IDE.

## Архитектура
Internet → Nginx/reverse proxy → FastAPI → worker → external APIs/sites.
FastAPI/worker → PostgreSQL.

## Стек
Linux, SSH, Docker, Docker Compose, PostgreSQL, Nginx, systemd или cron, Git, environment variables. CI/CD — по желанию.

## Изучить
Linux: filesystem, processes, permissions, environment variables, ports, SSH, logs.

Docker: image, container, volume, network, Dockerfile, Compose.

Deployment: git → build → deploy → start → logs → update.

Надёжность: health check, timeouts, retries, graceful failure, backup basics, secrets вне Git.

## Процесс
1. Dockerize приложение.
2. Проверить воспроизводимый local deployment.
3. Развернуть небольшой Linux VPS.
4. Настроить reverse proxy и HTTPS.
5. Добавить health endpoint и полезные logs.
6. Проверить восстановление после restart.
7. Документировать update procedure.

## Definition of Done
- [ ] Dockerfile;
- [ ] docker-compose.yml;
- [ ] PostgreSQL;
- [ ] environment variables;
- [ ] secrets не в Git;
- [ ] Linux VPS;
- [ ] SSH deployment;
- [ ] reverse proxy;
- [ ] HTTPS;
- [ ] health check;
- [ ] logs;
- [ ] deployment README.

## Не делать
Kubernetes, сложную cloud architecture, микросервисы, multi-region и autoscaling.

## Переход
Проект можно показать клиенту или работодателю: понятны проблема, решение, архитектура, запуск и ограничения.
