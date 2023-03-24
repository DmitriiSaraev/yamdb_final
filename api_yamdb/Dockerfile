FROM python:3.7-slim

# Сделать директорию /app рабочей директорией.
WORKDIR /app

# Скопировать с локального компьютера файл зависимостей
COPY requirements.txt .

# Выполнить установку зависимостей внутри контейнера.
RUN pip3 install -r /app/requirements.txt --no-cache-dir

# Скопировать в директорию .
COPY ./ .

# Выполнить запуск сервера разработки при старте контейнера.
CMD ["gunicorn", "api_yamdb.wsgi:application", "--bind", "0:8000" ]