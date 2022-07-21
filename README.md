# API YAMDB

## Описание

Этоn проект дает возможность людям делиться отзывами о различных фильмах,
книгах, музыкальных коллекциях и т.д.

## Документация REDOC

http://127.0.0.1:8000/redoc/

## Этот проект позволит Вам:

- Добавлять, просматривать, редактировать и удалять отзывы о произведениях.
- Добавлять, просматривать, редактировать и удалять комментарии к отзывам
  произведений.
- Ставить оценку произведениям от 1 до 10.

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/KuchishkinM/api_yamdb
```

```
cd api_yamdb
```

Cоздать и активировать виртуальное окружение:

```
python -m venv venv
```

```
source venv/Scripts/activate
```

```
python -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python manage.py migrate
```

Загрузить БД данными:

```
python manage.py import_db
```

Запустить проект:

```
python manage.py runserver
```

## Что использовалось для создания проекта:

- Python
- Django
- Django REST framework
- JWT token
- SQLite

## Авторы:

- Надежда Шестёра
- Алексей Чиненков
- Максим Кучишкин