
# VanillaNodeJSRestAPI

## Описание проекта
**VanillaNodeJSRestAPI** — это REST API, разработанный на чистом Node.js без использования фреймворков. Проект предоставляет базовый пример, демонстрирующий, как можно построить API с CRUD-операциями.

## Установка

1. Склонируйте репозиторий:
   ```bash
   git clone https://github.com/hayaSanzh/VanillaNodejsRestAPI.git
   cd VanillaNodejsRestAPI
   ```

2. Установите зависимости:
   ```bash
   npm install
   ```

## Запуск

Для запуска сервера используйте команду:
```bash
node server.js
```

API будет доступно по адресу: `http://localhost:3000`.

## Использование API

Примерные конечные точки:
- `GET /items` — получить список всех элементов
- `POST /items` — создать новый элемент
- `GET /items/:id` — получить элемент по ID
- `PUT /items/:id` — обновить элемент по ID
- `DELETE /items/:id` — удалить элемент по ID

## Примеры запросов

### Получить все элементы
```bash
curl -X GET http://localhost:3000/items
```

### Создать новый элемент
```bash
curl -X POST http://localhost:3000/items -d '{"name": "New Item", "description": "Description"}' -H "Content-Type: application/json"
```

### Получить элемент по ID
```bash
curl -X GET http://localhost:3000/items/1
```

### Обновить элемент
```bash
curl -X PUT http://localhost:3000/items/1 -d '{"name": "Updated Item"}' -H "Content-Type: application/json"
```

### Удалить элемент
```bash
curl -X DELETE http://localhost:3000/items/1
```

## Зависимости
- **Node.js** — JavaScript runtime для сервера
- **npm** — менеджер пакетов для управления зависимостями

## Лицензия
Этот проект лицензируется на условиях MIT.
