# API цитат - nestjs-quotes-api
Докеризированная версия проекта доступна в `feature/dockerize`

## Описание
Пример простого API сервиса цитат на Nest.js

Цитаты для упрощения реализации статически задаются в коде контроллера.

Используется в качестве демонстрационного сервиса в уроке по докеризации приложений.

# Документация
Автодокументация доступна по / и /docs

## Сборка
Без Docker: `npm ci && npm run build`

## Запуск
`npm run start`


docker build . -t nestjs-quotes-api:node20-alpine
docker run -p 3000:3000 nestjs-quotes-api:node20-alpine
docker image tag nestjs-quotes-api:node20-alpine sinitsabogdan/nestjs-quotes-api:node20-alpine
docker image push sinitsabogdan/nestjs-quotes-api:node20-alpine