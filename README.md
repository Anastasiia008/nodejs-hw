# nodejs-hw

Express-сервер для роботи з нотатками (гілка `01-express`).

## Запуск

```bash
npm install
cp .env.example .env
npm run dev   # розробка (nodemon)
npm start     # продакшн
```

## Маршрути

| Метод | Шлях | Відповідь |
|---|---|---|
| GET | `/notes` | 200 `{ "message": "Retrieved all notes" }` |
| GET | `/notes/:noteId` | 200 `{ "message": "Retrieved note with ID: <noteId>" }` |
| GET | `/test-error` | 500 `{ "message": "Simulated server error" }` |
| * | будь-який інший | 404 `{ "message": "Route not found" }` |
