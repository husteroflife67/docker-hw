Счётчик в Docker

Создай .env из примера.

cp .env.example .env

В .env можно поменять APP_PORT (порт на компьютере) и GREETING (текст приветствия).
По умолчанию счётчик открывается на http://127.0.0.1:8080/.

Запуск с Redis

docker compose up -d --build --wait

Остановка

docker compose down

Для варианта с SQLite используется другой файл

docker compose -f compose.sqlite.yaml up -d --build

Остановка SQLite

docker compose -f compose.sqlite.yaml down

Команды проверок, логи и ответы счётчика собраны в REPORT.txt.
