![test](https://github.com/DmitriiSaraev/yamdb_final/actions/workflows/yamdb_workflow.yaml/badge.svg)
# api_yamdb

api_yamdb
REST API для сервиса YaMDb — базы отзывов о фильмах, книгах и музыке. (Совместный проект 3 студентов Яндекс.Практикум)

Описание
API для сервиса YaMDb. Позволяет работать со следующими сущностями:

Отзывы (Получить список всех отзывов, создать новый отзыв, получить отзыв по id, частично обновить отзыв по id, удалить отзыв по id)

Коментарии к отзывам (Получить список всех комментариев к отзыву по id, создать новый комментарий для отзыва, получить комментарий для отзыва по id, частично обновить комментарий к отзыву по id, удалить комментарий к отзыву по id)

JWT-токен (Отправление confirmation_code на переданный email, получение JWT-токена в обмен на email и confirmation_code)

Пользователи (Получить список всех пользователей, создание пользователя, получить пользователя по username, изменить данные пользователя по username, удалить пользователя по username, получить данные своей учетной записи, изменить данные своей учетной записи)

Категории (типы) произведений (Получить список всех категорий, создать категорию, удалить категорию)

Категории жанров (Получить список всех жанров, создать жанр, удалить жанр)

Произведения, к которым пишут отзывы (Получить список всех объектов, создать произведение для отзывов, информация об объекте, обновить информацию об объекте, удалить произведение)

Полная документация API (redoc.yaml)
Клонировать репозиторий и перейти в него в командной строке

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```