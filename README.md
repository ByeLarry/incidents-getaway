# API-шлюз

## Описание

Данный репозиторий содержит реализацию API-шлюза, входящего в состав проекта ***incidents***.
API-шлюз выступает в качестве посредника между клиентской частью приложения и микросервисами. 
Помимо проксирования запросов, в задачи шлюза входит логирование, обеспечения связи независимых микросервисов и логика авторизации.

## Установка

```bash
# Установка зависимостей
npm install

# Запуск в dev режиме
npm run start:dev

# Запуск Redis
docker-compose up -d
```

## Проектирование

Стоит отметить, что в логике авторизации и логике входа в аккаунт сервер рассматривается как савокупность API-шлюза и микросервиса авторизации.

_Диаграммы можно сохранять и редактировать в ***[draw.io](https://app.diagrams.net/)***_

- ### Логика авторизации
  ![Логика авторизации](https://github.com/ByeLarry/incidents-getaway/assets/120035099/a7467b8d-0d3c-4563-a24b-e962d6c93431)

- ### Логика входа в аккаунт
  ![Отношение сущностей (точки)](https://github.com/user-attachments/assets/f81acef5-7118-4570-a3b9-71e3936d6fd9)

## Документация API
![image](https://github.com/user-attachments/assets/9c59f42f-6cbd-43de-8435-78274efe1bd2)


