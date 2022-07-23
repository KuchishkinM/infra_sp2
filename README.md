# Infra_sp2

## Описание

Этоn проект дает возможность людям делиться отзывами о различных фильмах,
книгах, музыкальных коллекциях и т.д.

## Документация REDOC

http://localhost/redoc/

## Этот проект позволит Вам:

- Добавлять, просматривать, редактировать и удалять отзывы о произведениях.
- Добавлять, просматривать, редактировать и удалять комментарии к отзывам
  произведений.
- Ставить оценку произведениям от 1 до 10.

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/KuchishkinM/infra_sp2
```

```
cd infra_sp2

```
Загрузить БД данными:

```
python manage.py import_db
```

Запустить docker-compose:

```
docker-compose up -d --build 
```


Выполнить миграции:

```
docker-compose exec web python manage.py migrate
```

Создать суперпользователя:

```
docker-compose exec web python manage.py createsuperuser
```

Подгрузить статику:

```
docker-compose exec web python manage.py collectstatic --no-input 
```

Загрузить БД данными:

```
docker-compose exec web python manage.py import.db
```

## Что использовалось для создания проекта:

- Python
- Django
- Django REST framework
- JWT token
- PostgreSQL
- Docker
## Авторы:

- Максим Кучишкин
