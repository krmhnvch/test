Digital Store & Chat Hub

Структура:
- main.py — FastAPI backend, авторизация, WebSocket-чат, загрузка изображений и настройки.
- requirements.txt — зависимости Python.
- Procfile — команда запуска для Railway/совместимого хостинга.
- templates/index.html — главная страница и встроенный чат.
- templates/chat_window.html — отдельное окно чата.
- templates/admin.html — панель администратора.
- static/uploads/ — загруженные изображения.

Локальный запуск:
1. Установить Python 3.10+ и PostgreSQL.
2. Создать виртуальное окружение: python -m venv .venv
3. Активировать окружение и установить зависимости: pip install -r requirements.txt
4. Задать переменные окружения DATABASE_URL и ADMIN_PASSWORD.
5. Запустить: uvicorn main:app --host 0.0.0.0 --port 8000

Открыть главную страницу по адресу http://localhost:8000, админ-панель — /admin.
Значения ADMIN_PASSWORD и DATABASE_URL обязательно задайте своими секретами перед публикацией.
